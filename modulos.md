Device Drivers  ---> 
   Generic Driver Options  --->                                   │
	[*] Maintain a devtmpfs filesystem to mount at /dev             │
 	[*] Select only drivers that don't need compile-time external fir
 	[*] Disable drivers features which enable custom firmware buildin  
	Firmware loader  --->    
 		-*- Firmware loading facility                          │
		[*]   Enable the firmware sysfs fallback mechanism       │
 	[*] Allow device coredump                                         │
   Bus devices  ----                                                │
	[*]   Report process events to userspace    
   -*- Plug and Play support  ---                                    │
   SCSI device support  --->                 
	{M} SCSI device support                                        │
	[*] SCSI: use blk-mq I/O path by default  
	<M> SCSI disk support                                          
	<M> SCSI generic support                                       │
	[*] Verbose SCSI error reporting (kernel size += 36K)          │
	[*] SCSI logging facility                                      │
	[*] Asynchronous SCSI scanning                                 │
	[*] SCSI low-level drivers  --->     
		[*]   LSI Logic New Generation RAID Device Drivers      │
	[*] SCSI Device Handlers  --->                                 │
X   <M> Serial ATA and Parallel ATA drivers (libata)  --->               │
 	[*]   ATA ACPI Support                                  │
 	[*]     SATA Zero Power Optical Disc Drive (ZPODD) support      │
 	[*]   SATA Port Multiplier support                               │
 	<M>   AHCI SATA support                                  │
     	(3)     Default SATA Link Power Management policy for mobile
 	<M>   ACard AHCI variant (ATP 8620)                         │
 	[*]   ATA SFF support (for legacy IDE and PATA)              │
           *** SFF controllers with custom DMA interface ***            │
 	[*]     ATA BMDMA support                                  │
           *** SATA SFF controllers with BMDMA ***  
   [*] Network device support  --->                               │
	[*]   Ethernet driver support  --->       
     		[*]   Realtek devices                            │
			<M>     Realtek 8169 gigabit ethernet support     │
	{M}   MDIO bus device drivers  ----           │
	{M}   PHY Device support and infrastructure  --->     │
		[*]   Support LED triggers for tracking link state    
		-M-   Realtek PHYs                         │
	[*]   ISDN support  --->                                  │
    Input device support  --->                                       │
 	-*- Generic input layer (needed for keyboard, mouse, ...)        │
 	{M}   Sparse keymap support library                              │
 	<M>   Event interface                                            │
 	[*]   Keyboards  --->                                            │
 		<*>   AT keyboard                         │
 	Hardware I/O ports  --->                                     │
		-*- Serial I/O support                                    │
 		-*- i8042 PC Keyboard controller  
		-*- PS/2 driver library                                   │
 		<M> Raw access to serio ports
    Character devices  --->                                          │
 	[*] Enable TTY                                                   │
 	[*]   Virtual terminal                                           │
 	[*]     Enable character translations in console                 │
 	[*]     Support for console on virtual terminal                  │
 	-*-     Support for binding and unbinding console drivers        │
 	[*]   Unix98 PTY support                                         │
 	[*]   Non-standard serial port support                           │
 	[*]   Automatically load TTY Line Disciplines                    │
 	[*] /dev/mem virtual device support                              ││
	Serial drivers  --->                                         │
		<*> 8250/16550 and compatible serial support             │
		[*]   8250/16550 PNP device support              │
		[*]   Support for Fintek F81216A LPC to 4 UART RS485 API
		[*]   Console on 8250/16550 and compatible serial port│
		[*]   DMA support for 16550 compatible UART controllers
		<*>   8250/16550 PCI device support
		[*]   Extended 8250/16550 serial driver options            
		[*]     Support more than 4 legacy serial ports │ 
		[*] Support for sharing serial interrupts               
		[*] Support RSA serial ports                  │
		<*> Support for Synopsys DesignWare 8250 quirks        
		<*> Support for serial ports on Intel MID platforms     
	<*> Serial device bus  --->                                      │
 		[*]   Serial device TTY port controller                 │
	[*] Xen Hypervisor Console support                               │
 	[*]   Xen Hypervisor Multiple Consoles support                   │
	{M} Hardware Random Number Generator Core support  --->          │
	[*] HPET - High Precision Event Timer                            │
 	[*]   Allow mmap of HPET                                         │
 	[*]     Enable HPET MMAP access by default                         
	[*] /dev/port character device                          │
   I2C support  --->                                                │
	<*> I2C support                                               │
 	[*]   ACPI I2C Operation region support                       │
 	[*]   Enable compatibility bits for old user-space            │   		<M>   I2C bus multiplexing support                            │
	[*]   Autoselect pertinent helper modules                     │
 	I2C Hardware Bus support  --->  
		<M> Intel PIIX4 and compatible (ATI/AMD/Serverworks/Broadcom/SMSC
		-*- Synopsys DesignWare Platform 
		[*] Intel Baytrail I2C semaphore support          │
   -*- PPS support  --->                             │
   PTP clock support  --->                                          │
	<*> PTP clock support 
   -*- Pin controllers  --->
	<*>   AMD GPIO pin control
   -*- GPIO Support  --->
   -*- Power supply class support  --->
   -*- Generic Thermal sysfs driver  --->	
	Default Thermal governor (step_wise)  --->
		<X> step_wise
   Multifunction device drivers  --->                               │
	[*] Support for Intel Cherry Trail Whiskey Cove PMIC
   Graphics support  --->
	Frame buffer Devices  --->
		<*> Support for frame buffer devices  ---> 
		[*] Enable Video Mode Handling Helpers
		[*] Enable Tile Blitting Support
		[*] VESA VGA graphics support
		[*] EFI-based Framebuffer Support 
		<*> Xen virtual frame buffer support
	[*] Backlight & LCD device support  --->
		<*>   Lowlevel Backlight controls
	Console display driver support  --->
		[*] VGA text console
		[*] Framebuffer Console support                 
		[*]   Map the console to the primary display device
		[*]   Framebuffer Console Rotation
   HID support  --->
	{M} HID bus support
	[*]   Battery level reporting for HID devices                  │
	[*]   /dev/hidraw raw HID device support                       │
	<M>   Generic HID driver                                       │
	Special HID drivers  --->
	USB HID support  --->
		<M> USB HID transport layer
		[*] PID device support                                  │
		[*] /dev/hiddev raw HID device support
	I2C HID support  --->
		<M> HID over I2C transport layer
+   [*] USB support  --->
	<M>   Support for Host-side USB
	[*]   PCI based USB host interface
	[*]   USB announce new devices
	[*]   Enable USB persist by default
	[*]   Dynamic USB minor allocatio
	<M>   xHCI HCD (USB 3.0) support
	<M>   EHCI HCD (USB 2.0) support
	[*]     Root Hub Transaction Translators
	[*]     Improved Transaction Translator scheduling
	[*]   USB LED Triggers
   [*] LED Support  --->                                                │
	<*>   LED Class Support 
	[*]     LED Class brightness_hw_changed attribute support
	[*]   LED Trigger support  --->
		[*]   LED CPU Trigger
		[*]   LED Panic Trigger
   [*] Accessibility support  --->
	[*]   Console on braille device
   <*> EDAC (Error Detection And Correction) reporting  --->            │
	[*]   EDAC legacy sysfs
	<M>   Decode MCEs in human-readable form (only on AMD for now)
   [*] Real Time Clock  --->                                            │
	[*]   Set system time from RTC on startup and resume  
	[*]   Set the RTC time based on NTP synchronization
	[*]   RTC non volatile storage support
	[*]   /sys/class/rtc/rtcN (sysfs)
	[*]   /proc/driver/rtc (procfs for rtcN)
	<*>   PC-style 'CMOS'
   -*- DMA Engine support  --->                                         │
	[*]   Async_tx: Offload support for the async_tx api           │
   DMABUF options  --->                                             │
	[*] Explicit Synchronization Framework                  │
   [*] Virtualization drivers  --->                                     
   [*] Virtio drivers  --->                                             │
   Xen driver support  --->                                         │
	[*] Xen memory balloon driver
	[*]   Memory hotplug support for Xen balloon driver
	[*]   Scrub pages before returning them to system by default
	[*] Backend driver support
	[*] Create xen entries under /sys/hypervisor
	[*] Xen platform mcelog 
   [*] Staging drivers  --->                                            │
	[*]   Media staging drivers  ----                              │
   [*] X86 Platform Specific Device Drivers  --->                       │
	<M>   Lenovo IdeaPad Laptop Extras  
	<M>   WMI
	<M>     WMI embedded Binary MOF driver
   [*] Platform support for Chrome hardware  --->
   -*- Mailbox Hardware Support  --->
	-*-   Platform Communication Channel Driver
   [*] IOMMU Hardware Support  --->                                     │
	[*]   AMD IOMMU support
	<*>     AMD IOMMU Version 2 driver
	[*]   Support for Intel IOMMU using DMA Remapping Devices
	[*]     Support for Shared Virtual Memory with Intel IOMMU        │
	[*]   Support for Interrupt Remapping
   [*] Generic Dynamic Voltage and Frequency Scaling (DVFS) support     │
   [*] Memory Controller drivers  ----
   [*] Pulse-Width Modulation (PWM) Support  --->
   PHY Subsystem  ---> 
	[*] PHY Core 
   [*] Generic powercap sysfs driver  ---> 
   -*- Reliability, Availability and Serviceability (RAS) features      │
   Android  --->
	[*] Android Drivers
   -*- DAX: direct access to differentiated memory  --->
   -*- NVMEM Support  ----                                              │

File systems  --->
   <M> The Extended 4 (ext4) filesystem                               │
   [*]   Use ext4 for ext2 file systems
   [*]   Ext4 POSIX Access Control Lists
   [*]   Ext4 Security Labels
   [*]   Ext4 Encryption
   <M> Btrfs filesystem support                                       │
   [*]   Btrfs POSIX Access Control Lists
   [*] Direct Access (DAX) support 
   -*- Enable filesystem export operations for block IO 
   [*] Enable POSIX file locking API                                  │
   [*]   Enable Mandatory file locking                                │
   {M} FS Encryption (Per-file encryption)                            │
   [*] Dnotify support                                                │
   [*] Inotify support for userspace                                  │
   [*] Filesystem wide access notification                            │
   [*]   fanotify permissions checking                                │
   [*] Quota support                                                  │
   [*] Report quota messages through netlink interface                │
   [*] Print quota warnings to console (OBSOLETE)
   <M> Kernel automounter support (supports v3, v4 and v5)            │
   <M> FUSE (Filesystem in Userspace) support
   DOS/FAT/NT Filesystems  --->
	<M> VFAT (Windows-95) fs support                         │
	[*]   Enable FAT UTF-8 option by default
   Pseudo filesystems  --->                                       │
	[*] /proc file system support
	[*]   /proc/kcore support
	[*]   /proc/vmcore support                                         		[*]   Sysctl support (/proc/sys) 
	-*-   Enable /proc page monitoring                                 		-*- Include /proc/<pid>/task/<tid>/children file
	[*] sysfs file system support
	[*] Tmpfs virtual memory file system support (former shm fs)       		[*]   Tmpfs POSIX Access Control Lists                             		-*-   Tmpfs extended attributes                                    		[*] HugeTLB file system support                                    		<M> EFI Variable filesystem
   -*- Miscellaneous filesystems  --->
	<M>   SquashFS 4.0 - Squashed file system support
	File decompression options (Decompress file data into an
		<X> Decompress file data into an intermediate buffer
        Decompressor parallelisation options (Single threaded com
		<X> Single threaded compression
	[*]     Squashfs XATTR support	
	[*]     Include support for ZLIB compressed file systems
	[*]     Include support for LZ4 compressed file systems
 	[*]     Include support for LZO compressed file systems
 	[*]     Include support for XZ compressed file systems
 	[*]     Include support for ZSTD compressed file systems
	-*-   Persistent store support
	<*>     DEFLATE (ZLIB) compression
	Default pstore compression algorithm (deflate)  --->
		<X> deflate                               │
   [*] Network File Systems  --->                                     │
	<M>   NFS server support
	-*-     NFS server support for NFS version 3
	[*]       NFS server support for the NFSv3 ACL protocol extension
	[*]     NFS server support for NFS version 4
	[*]   NFSv4.1 server support for pNFS block layouts
	[*]   Provide Security Label support for NFSv4 server
	[*]   RPC: Enable dprintk debugging
   -*- Native language support  --->
	<M>   Codepage 437 (United States, Canada)
	<M>   ASCII (United States)




Security options  --->  
   -*- Enable access key retention support
   [*]   Diffie-Hellman operations on retained keys                     │
   [*] Restrict unprivileged access to the kernel syslog                │
   [*] Restrict unprivileged use of performance events                  │
   [*] Enable different security models                                 │
   -*- Enable the securityfs filesystem                                 │
   -*- Socket and Networking Security Hooks                             │
   [*] Remove the kernel mapping in user mode                           │
   -*- Security hooks for pathname based access control
   [*] Harden memory copies between kernel and userspace                │
   [*] Harden common str/mem functions against buffer overflows         │
   -*- Allow the kernel to be 'locked down'                             │
   [*] Lock down the kernel in EFI Secure Boot mode                     │
   [*] NSA SELinux Support
   [*]   NSA SELinux Development Support                                │
   [*]   NSA SELinux AVC Statistics
   [*] TOMOYO Linux Support                                             │
   [*]   Enable introspection of sha1 hashes for loaded profiles        │
   [*]     Enable policy hash introspection by default
   [*] Yama support                                                     │
   [*] Integrity subsystem                                              │
   [*]   Digital signature verification using multiple keyrings         │
   [*]     Enable asymmetric keys support                               │
   [*]   Enables integrity auditing support
   Default security module (AppArmor)  --->                         │
	<X> AppArmor


-*- Cryptographic API  --->                                  │
   [*]   FIPS 200 compliance                                            │
   -*-   RSA algorithm                                                  │
   -*-   Diffie-Hellman algorithm                                       │
   <M>   ECDH algorithm                                                 │
   -*-   Cryptographic algorithm manager                                │
   {M}   GF(2^128) multiplication functions                             │
   {M}   Null algorithms                                                │
   {M}   Software async crypto daemon
   <M>   CCM support                                                    │
   <M>   GCM/GMAC support
   {M}   Sequence Number IV Generator                                   │
   {M}   CBC support
   {M}   CTR support                                                    │
   {M}   CTS support                                                    │
   {M}   ECB support                                                    │
   {M}   XTS support                                                    │
   <M>   CMAC support                                                   │
   {*}   HMAC support                                                   │
   {M}   CRC32c CRC algorithm                                           │
   <M>   CRC32c INTEL hardware acceleration                             │
   <M>   CRC32 PCLMULQDQ hardware acceleration                          │
   -*-   CRCT10DIF algorithm
   <M>   CRCT10DIF PCLMULQDQ hardware acceleration                      │
   {M}   GHASH digest algorithm                                         │
   <*>   MD5 digest algorithm                                           │
   -*-   SHA1 digest algorithm                                          │
   -*-   SHA224 and SHA256 digest algorithm
   <M>   GHASH digest algorithm (CLMUL-NI accelerated)                  │
   -*-   AES cipher algorithms                                          │
   {M}   AES cipher algorithms (x86_64)                                 │
   <M>   AES cipher algorithms (AES-NI)                                 │
   <M>   ARC4 cipher algorithm
   -*-   Deflate compression algorithm                                  │
   -*-   LZO compression algorithm
   <M>   Pseudo Random Number Generation for Cryptographic modules      │
   {M}   NIST SP800-90A DRBG  --->
*
*
*
*
*
*
*



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

