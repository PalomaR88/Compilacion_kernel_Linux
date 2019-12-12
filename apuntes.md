# Kernel Linux

### Características principales
- Kérnel del sistema GNU/Linux, licenciado bajo GNU GPL. 
- Desarrollo colaborativo de miles de personas
- Monolítico
- LKM: loadable kernel module
- Última versión estable: 5.3.5. Pero este kernel no es que tiene la última actualización de Debian, sino que se usan los longterm porque son más seguros. 
- kernel.org
- Portado a gran cantidad de arquitecturas, desde pequeños dispositivos a grandes supercomputadores.


### Características de compilación
El codigo fuente de rama vanila del núcleo ocupa actualmente 886MiB (cuando se hizo la diapositiva, ahora será más).

Los componentes del kérnel se compilan de dos formas:
- Enlace estática: Se incluyen dentro de un fichero ejecutable enlazado estáticamente y que habitualmente se denomina vmlinuz o zlmage.
- Enlace dinámico: Se compilan individualmente en ficheros objetos con extensión .ko que se cargan en memoria a demanda (están ubicados en /lib/modules).

Los módulos son fragmentos del kernel que se cargan dinámicamente. Debian, algunos de estos módulos los ha quitado del su kernel, pero se pueden compilar.

Hay 3 tipos de ficheros:
- Fuente: con extensión .c(del lenguaje C)
- Objeto: con extensión .o -> .ko
- Binario: sin extensión.

Soluciones para hardware no detectado en el arranque:
- Se aumenta el tamaño del fichero ejecutable (bzlmage o big zlmage)
- Se montan temporalmente algunos módulos en memoria (initramfs)

Distribución de uso general en sistemas x86:
- Enorme variedad de hardware.
- Se incluyen gran cantidad de 

~~~
file initrd.img-4.19.0-6amd64
du -hs /lib/modules/4.19.0-6-amd64/
~~~

# Compilación
### Manejo de módulos
Para ver los módulos adicionales que está usando la máquina, normalmente por hardware:
~~~
lsmod
lsmod | wc -l 
~~~

Algunos ejemplos de módulos:
snd_hda_codec -> tarjetas de sonido
parport_pc -> soporte para puerto paralelo (este no lo suele tener los portátiles)

Quitar modulos de la memoria:
~~~
modprobe -r <nombre del módulo>
~~~

~~~
find /home/`whoami` -type f -iname vagrantfile
~~~

~~~
/lib/modules/4.19.0-6-amd64/<kernel>
~~~

hid: driver de dispositivos con interaccion con humanos. 
infiniband: tarjeta de alta capacidad.
mISDN: tipo de conexión antes que el ADSL.
leds: leds


Esta es la configuración final que ha realizado Debian.
~~~
/boot/config-4.19.0-6-amd64
~~~

Cuando aquí encuentras =m es que es un módulo, y lo compila dinámicamente. 
~~~
grep "=m" /boot/config-4.19.0-6-amd64 | wc -l
~~~

Para que aparezcan todos los módulos. 
~~~
sudo find /lib/modules/4.19.0-6-amd64/ -type f -iname '*.ko'
~~~

Módulos cargados:
~~~
lsmod
~~~

Carga el módulo en memoria:
~~~
modprobe <módulo>
~~~
Descarga el módulo de la memoria:
~~~
modprobe -r <módulo>
~~~

Módulos disponibles:
~~~
find /lib/modules/'uname -r' -type f -iname '*.ko
~~~

Información del módulo
~~~
modinfo <módulo>
~~~

Actualiza las dependencias de los módulos
~~~
depmod
~~~


### Instalación

~~~
$ sudo apt update
$ sudo apt install linux-source-4.9
~~~

Se descomprime el fichero .tar que se crea en /usr/src/ en el directorio donde se quiere trabajar:
~~~
$ tar -xf /usr/src/linux-source-4.19.tar.xz 
~~~

Se copia el fichero .config que se usa actualmente:
~~~
$ cp /boot/config-4.19.0-6-amd64 ./.config
~~~

> Para cambiar el nombre de las compilaciones que se van a realizar del kernel y, por tanto, tener un control de las diferentes versiones, se modifica el fichero Makefile en la línea EXTRAVERSION.
~~~
# SPDX-License-Identifier: GPL-2.0
VERSION = 4
PATCHLEVEL = 19
SUBLEVEL = 67
EXTRAVERSION = -1
NAME = "People's Front"
~~~



### Primera configuración del kernel - Adaptación a la máquina
Con la opción localmodconfig se configura el fichero .config adaptandolo a las necesidades de nuetra máquina. 
~~~
$ make localmodconfig
~~~

### Configuración de .config
Esta configuración se puede hacer con las siguientes bibliotecas de desarrollo:
- menuconfig (este es el que vamos a utilizar)
~~~
sudo apt-get install libncurses5-dev
make nconfig
~~~

- gconfig
~~~
sudo apt-get install libgtk2.0-dev libglib2.0-dev libglade2-dev
make gconfig
~~~

-xconfig
~~~
sudo apt-get install libqt4-dev
make xconfig
~~~

### Compilación, último paso
Para compilar se usa el siguiente comando:
~~~
$ make -j2 deb-pkg
~~~

> **-j** es para indicar los núcleos que usaremos para la compilación.
 
