Device Drivers  ---> 
   Generic Driver Options  --->                                     │
 │ 	[ ] Support for uevent helper                                  │
 │ 	[*] Maintain a devtmpfs filesystem to mount at /dev             │
 │ 	[ ]   Automount devtmpfs at /dev, after the kernel mounted the ro 
 │ 	[*] Select only drivers that don't need compile-time external fir
 │ 	[*] Disable drivers features which enable custom firmware buildin  │ │     Firmware loader  --->    
 │ 		-*- Firmware loading facility                          │
 │     		()    Build named firmware blobs into the kernel binary 
		[*]   Enable the firmware sysfs fallback mechanism       │
 │ 		[ ]     Force the firmware sysfs fallback mechanism when possible │
 │ 	[*] Allow device coredump                                         │
 │ 	[ ] Driver Core verbose debug messages                          │
 │ 	[ ] Managed device resources verbose debug messages               │
 │ 	[ ] Test driver remove calls during probe (UNSTABLE)              │
 │ 	< > Build kernel module to test asynchronous driver probing       │
 │ 	[ ] Enable verbose DMA_FENCE_TRACE messages   
   Bus devices  ----                                                │
 │ <*> Connector - unified userspace <-> kernelspace linker  --->  │
	[*]   Report process events to userspace    
 │ < > GNSS receiver support  ----                             │
 │ < > Memory Technology Device (MTD) support  ----                     │
 │ [ ] Device Tree and Open Firmware support  ----                      │
 │ < > Parallel port support  ----                                      │
 │ -*- Plug and Play support  --->      
    [ ]   PNP debugging messages                       │
 │                         *** Protocols ***                            │
 │ [ ] Block devices  ----                                              │
 │     NVME Support  ---> 
*
*
*
*
*                                              │
 │     Misc devices  --->                                               │
 │ < > ATA/ATAPI/MFM/RLL support (DEPRECATED)  ----                     │
 │     SCSI device support  --->                                        │
 │ <M> Serial ATA and Parallel ATA drivers (libata)  --->               │
 │ [ ] Multiple devices driver support (RAID and LVM)  ----             │
 │ < > Generic Target Core Mod (TCM) and ConfigFS Infrastructure  --    │
 │ [ ] Fusion MPT device support  ----                                  │
 │     IEEE 1394 (FireWire) support  --->                               │
 │ [ ] Macintosh device drivers  ----                                   │
 │ [*] Network device support  --->                                     │
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
