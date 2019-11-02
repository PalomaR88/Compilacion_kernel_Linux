Device Drivers  ---> 
   
 │ [*] Block devices  --->                                              │


 ┌── Serial ATA and Parallel ATA drivers (libata) ──────────────────────┐

 │ [ ]   Verbose ATA error reporting                                    │


 ┌── Multiple devices driver support (RAID and LVM) ────────────────────┐
 │                                                                      │
 │        --- Multiple devices driver support (RAID and LVM)            │
 │        < >   RAID support                                            │
 │        < >   Block device as cache                                   │
 │        < >   Device mapper support  

 │ [ ] Fusion MPT device support  ----                                  │

 │ [ ] Macintosh device drivers  ----                                   │


 ┌── Network device support ────────────────────────────────────────────┐
 │                                                                      │
 │ --- Network device support                                           │
 │ [ ]   Network core driver support                                    │
 │ < >   ARCnet support  ----                                           │
 │       *** CAIF transport drivers ***                                 │
 │       Distributed Switch Architecture drivers  ----                  │
 │ [*]   Ethernet driver support  --->   

── Ethernet driver support ───────────────────────────────────────────┐
 │                                                                      │
 │ [ ]   OKI Semiconductor devices                                      │
 │ < >   OpenCores 10/100 Mbps Ethernet MAC support                     │
 │ [ ]   Packet Engine devices                                          │
 │ [ ]   QLogic devices                                                 │
 │ [ ]   Qualcomm devices                                               │
 │ [ ]   RDC devices                                                    │
 │ [*]   Realtek devices                                                │
 │ < >     RealTek RTL-8139 C+ PCI Fast Ethernet Adapter support        │
 │ < >     RealTek RTL-8129/8130/8139 PCI Fast Ethernet Adapter supp    │
 │ <M>     Realtek 8169 gigabit ethernet support 


 ┌── Pin controllers ───────────────────────────────────────────────────┐
 │                                                                      │
 │      --- Pin controllers                                             │
 │      [ ]   Debug PINCTRL calls                                       │
 │      <*>   AMD GPIO pin control                                      │
 │      < >   Microchip MCP23xxx I/O expander                           │
 │      [ ]   Semtech SX150x I2C GPIO expander pinctrl driver           │
 │      [*]   Intel Baytrail GPIO pin control                           │
 │      <*>   Intel Cherryview/Braswell pinctrl and GPIO driver         │
 │      <*>   Intel Broxton pinctrl and GPIO driver                     │
 │      <*>   Intel Cannon Lake PCH pinctrl and GPIO driver             │
 │      <*>   Intel Cedar Fork pinctrl and GPIO driver                  │
 │      <*>   Intel Denverton pinctrl and GPIO driver                   │
 │      <*>   Intel Gemini Lake SoC pinctrl and GPIO driver             │
 │      <*>   Intel Ice Lake PCH pinctrl and GPIO driver                │
 │      <*>   Intel Lewisburg pinctrl and GPIO driver                   │
 │      <*>   Intel Sunrisepoint pinctrl and GPIO driver                │
 │                                                         

 ┌── GPIO Support ──────────────────────────────────────────────────────┐
 │                                                                      │
 │          --- GPIO Support                                            │
 │              (512) Maximum number of GPIOs for fast path             │
 │          [ ]   Debug GPIO calls                                      │
 │          [*]   /sys/class/gpio/... (sysfs interface)                 │
 │                Memory mapped GPIO drivers  --->                      │
 │                Port-mapped I/O GPIO drivers  --->                    │
 │                I2C GPIO expanders  --->                              │
 │                MFD GPIO expanders  ----                              │
 │                PCI GPIO expanders  --->                              │
 │                SPI GPIO expanders  --->                              │
 │                USB GPIO expanders  ----                              │
 │                                                                      │

 │ {*} Hardware Monitoring support  --->    
 │ 	< >   AMD Family 10h+ temperature sensor                             │
 │ 	< >   AMD Family 15h processor power   


┌── Generic Thermal sysfs driver ──────────────────────────────────────┐
 │                                                                      │
 │        --- Generic Thermal sysfs driver                              │
 │        [*]   Thermal state transition statistics                     │
 │            (0)   Emergency poweroff delay in milli-seconds           │
 │        [*]   Expose thermal sensors as hwmon device                  │
 │        [*]   Enable writable trip points                             │
 │              Default Thermal governor (step_wise)  --->              │
 │        [*]   Fair-share thermal governor                             │
 │        -*-   Step_wise thermal governor                              │
 │        [*]   Bang Bang thermal governor                              │
 │        [*]   User_space thermal governor                             │
 │        [ ]   Power allocator thermal governor                        │
 │        [ ]   Generic clock cooling support                           │
 │        [*]   Generic device cooling support                          │
 │        [ ]   Thermal emulation mode support                          │
 │        < >   Intel PowerClamp idle injection driver                  │
 │        < >   X86 package temperature thermal driver                  │
 │        < >   Intel SoCs DTS thermal driver                           │
 │              ACPI INT340X thermal drivers  --->                      │
 │        < >   Intel PCH Thermal Reporting Driver                      │

 │ [ ] Voltage and Current Regulator Support  ----                      │


 │ < > Multimedia support  ----                                         │

┌── Graphics support ──────────────────────────────────────────────────┐
 │                                                                      │
 │ <*> /dev/agpgart (AGP Support)  --->                                 │
 │ -*- VGA Arbitration                                                  │
 │     (16)  Maximum number of GPUs                                     │
 │ [*] Laptop Hybrid Graphics - GPU switching support                   │
 │ <M> Direct Rendering Manager (XFree86 4.1.0 and higher DRI suppor    │
 │ [*] Enable DisplayPort CEC-Tunneling-over-AUX HDMI support           │
 │     I2C encoder or helper chips  --->                                │
 │ < > ATI Radeon                                                       │
 │ <M> AMD GPU                                                          │
 │ [*]   Enable amdgpu support for SI parts                             │
 │ [*]   Enable amdgpu support for CIK parts                            │
 │ [*]   Always enable userptr write support                            │
 │ [ ]   Allow GART access through debugfs                              │
 │     ACP (Audio CoProcessor) Configuration  --->                      │
 │     Display Engine Configuration  --->                               │
 │     AMD Library routines  --->                                       │
 │ < > Nouveau (NVIDIA) cards                                           │
 │ < > Intel 8xx/9xx/G3x/G4x/HD Graphics                                │
 │ < > Virtual GEM provider                                             │
 │ < > Virtual KMS (EXPERIMENTAL)                                       │
 │ < > DRM driver for VMware Virtual GPU                                │
 │ < > Intel GMA5/600 KMS Framebuffer                                   │
 │ < > DisplayLink                                                      │
 │ < > AST server chips                                                 │
 │ < > Kernel modesetting driver for MGA G200 server engines            │
 │ < > Cirrus driver for QEMU emulated device                           │
 │ <M> HSA kernel driver for AMD GPU devices                            │
 │ < > DRM Support for Hisilicon Hibmc                                  │
 │ < > Support for simple displays  ----                                │
 │ [*] DRM Support for Xen guest OS                                     │
 │ < >   Para-virtualized frontend driver for Xen guest OS              │
 │ [*] Enable legacy drivers (DANGEROUS)  --->                          │
 │     Frame buffer Devices  --->                                       │
 │ -*- Backlight & LCD device support  --->                             │
 │     Console display driver support  --->                             │
 │ [ ] Bootup logo  ----                                                │










	Generic Driver Options  --->                                   │
 │ 	[*] Maintain a devtmpfs filesystem to mount at /dev             │
 │ 	[*] Select only drivers that don't need compile-time external fir
 │ 	[*] Disable drivers features which enable custom firmware buildin  │ │     Firmware loader  --->    
 │ 		-*- Firmware loading facility                          │
 │     		()    Build named firmware blobs into the kernel binary 
		[*]   Enable the firmware sysfs fallback mechanism       │
 │ 	[*] Allow device coredump                                         │
   Bus devices  ----                                                │
 │ <*> Connector - unified userspace <-> kernelspace linker  --->  │
	[*]   Report process events to userspace    
 │ -*- Plug and Play support  ---                                    │
 │     NVME Support  ---> 
	<M> NVM Express block device                              │
 │            [*] NVMe multipath support                           │
 │     SCSI device support  --->                 
         {M} SCSI device support                                        │
 │       [*] SCSI: use blk-mq I/O path by default                       │
 │           *** SCSI support type (disk, tape, CD-ROM) ***             │
 │       [*] Verbose SCSI error reporting (kernel size += 36K)          │
 │       [*] SCSI logging facility                                      │
 │       [*] Asynchronous SCSI scanning                                 │
 │       [*] SCSI low-level drivers  --->     
 │ 		[*]   LSI Logic New Generation RAID Device Drivers      │
 │ 		< >     LSI Logic Management Module (New Driver)        │
 │       [*] SCSI Device Handlers  --->                                 │
 │ <M> Serial ATA and Parallel ATA drivers (libata)  --->               │
	[*]   Verbose ATA error reporting                                 │
 │ 	[*]   ATA ACPI Support                                  │
 │ 	[*]     SATA Zero Power Optical Disc Drive (ZPODD) support      │
 │ 	[*]   SATA Port Multiplier support                               │
 │       *** Controllers with non-SFF native interface ***              │
 │ 	<M>   AHCI SATA support                                  │
 │     	(3)     Default SATA Link Power Management policy for mobile
 │ 	<M>   ACard AHCI variant (ATP 8620)                         │
 │ 	[*]   ATA SFF support (for legacy IDE and PATA)              │
 │         *** SFF controllers with custom DMA interface ***            │
 │ 	[*]     ATA BMDMA support                                  │
 │           *** SATA SFF controllers with BMDMA ***                    │
 │ [*] Network device support  --->                                     │
	[*]   Network core driver support                               │
 │ 	[*]     Fibre Channel driver support                              │
 │ 	[*]   Ethernet driver support  --->       
                [*]   3Com devices                                     │
 │ 		[*]   Adaptec devices                                   │
 │ 		[*]   Agere devices                            │
 │ 		[*]   Alacritech devices                           │
 │ 		[*]   Alteon devices                          ││
 │ 		[*]   Amazon Devices                                  │
 │ 		[*]   AMD devices                             │
 │ 		[*]   aQuantia devices                         │
 │ 		[*]   Atheros devices                        │
		[*]   Broadcom devices                           │
 │ 		[*]   QLogic BR-series devices                    │
		[*]   Cadence devices                             │
 │ │ 		[*]   Cavium ethernet drivers                      │
 │ 		<*>     Cavium PTP coprocessor as PTP clock          │
 │ 		[*]   Chelsio devices                        │
 │ 		[*]   Cisco devices                            │
		[*]   Cortina Gemini devices                    │
 │ 		[*]   Digital Equipment devices                           │
 │ 		[*]     DEC - Tulip devices                      │
 │ 		[*]   D-Link devices                           │
 │ 		[*]   Emulex devices                          │
 │ 		[*]   EZchip devices                             │
 │ 		[*]   HP devices                                    │
 │ 		[*]   Huawei devices                            │
 │ │ 		[*]   Intel (82586/82593/82596) devices            │
 │ 		[*]   Intel devices                             │
		[*]   Marvell devices                         │
 │ 		[*]   Mellanox devices                           │
 │ 		[*]   Micrel devices                               │
 │ 		[*]   Microchip devices                          │
 │ 		[*]   Microsemi devices                       │
 │ 		[*]   Myricom devices                              │
 │  		[*]   National Semiconductor devices                │
 │ 		[*]   Neterion (Exar) devices          
		[*]   Netronome(R) devices                         │
 │ 		[*]   National Instruments Devices                │
 │ 		[*]   National Semiconductor 8390 devices            │
 │  │ 		[*]   NVIDIA devices                         │
 │ 		[*]   OKI Semiconductor devices                           │
 │ 		[*]   Packet Engine devices                    │
 │ 		[*]   QLogic devices                      │
 │ 		[*]   Qualcomm devices                            │
 │ 		[*]   RDC devices                   │
 │ 		[*]   Realtek devices                          │
 │ 		<M>     Realtek 8169 gigabit ethernet support  
[*]   Renesas devices                                                │
 │ [*]   Rocker devices                                                 │
 │ [*]   Samsung Ethernet devices                                       │
 │ < >     Samsung 10G/2.5G/1G SXGBE Ethernet driver                    │
 │ [ ]   SEEQ devices                                                   │
 │ [*]   Solarflare devices                                             │
 │ < >     Solarflare SFC9000/SFC9100-family support                    │
 │ < >     Solarflare SFC4000 support                                   │
 │ [*]   Silan devices                                                  │
 │ < >     Silan SC92031 PCI Fast Ethernet Adapter driver               │
 │ [*]   Silicon Integrated Systems (SiS) devices                       │
 │ < >     SiS 900/7016 PCI Fast Ethernet Adapter support               │
 │ < >     SiS190/SiS191 gigabit ethernet support                       │
 │ [*]   SMC (SMSC)/Western Digital devices                             │
 │ < >     SMC EtherPower II                                            │
 │ < >     SMSC LAN911x/LAN921x families embedded ethernet support      │
 │ < >     SMSC LAN9420 PCI ethernet adapter support                    │
 │ [*]   Socionext ethernet drivers                                     │
 │ [*]   STMicroelectronics devices                                     │
 │ < >     STMicroelectronics 10/100/1000/EQOS Ethernet driver          │
 │ [*]   Sun devices    
*
*
*
*
*
*

 │ <*>   FDDI driver support                                            │
 │ < >     Digital DEFTA/DEFEA/DEFPA adapter support                    │
 │ < >     SysKonnect FDDI PCI support                                  │
 │ [*]   HIPPI driver support                                           │




 │ [ ] Open-Channel SSD target support  ----                            │
 │     Input device support  --->                                       │
 │     Character devices  --->                                          │
 │ [*] Trust the CPU manufacturer to initialize Linux's CRNG            │
 │     I2C support  --->                                                │
 │ [*] SPI support  --->                                                │
 │ < > SPMI support  ----                                               │
 │ < > HSI support  ---- 
│ -*- PPS support  --->                                                │
 │     PTP clock support  --->                                          │
 │ -*- Pin controllers  --->                                            │
 │ -*- GPIO Support  --->                                               │
 │ < > Dallas's 1-wire support  ----                                    │
 │ [ ] Adaptive Voltage Scaling class support  ----                     │
 │ [ ] Board level reset or power off  ----                             │
 │ -*- Power supply class support  --->                                 │
 │ <*> Hardware Monitoring support  --->                                │
 │ -*- Generic Thermal sysfs driver  --->                               │
 │ [*] Watchdog Timer Support  --->                                     │
 │ < > Sonics Silicon Backplane support  ----                           │
 │ < > Broadcom specific AMBA  ----                                     │
 │     Multifunction device drivers  --->                               │
 │ [ ] Voltage and Current Regulator Support  ----                      │
 │ < > Remote Controller support  ----                                  │
 │ < > Multimedia support  ----                                         │
 │     Graphics support  --->  

