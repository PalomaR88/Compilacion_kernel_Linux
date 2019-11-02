Device Drivers  ---> 
     ┌── Networking support ────────────────────────────────────────────────┐
 │                                                                      │
 │      --- Networking support                                          │
 │            Networking options  --->                                  │
 │      [*]   Amateur Radio support  --->                               │
 │      < >   CAN bus subsystem support  ----                           │
 │      <M>   Bluetooth subsystem support  --->                         │
 │      < >   RxRPC session sockets                                     │
 │      < >   KCM sockets                                               │
 │      [*]   Wireless  --->                                            │
 │      < >   WiMAX Wireless Broadband support  ----                    │
 │      <M>   RF switch subsystem support  --->                         │
 │      < >   Plan 9 Resource Sharing Support (9P2000)  ----            │
 │      < >   CAIF support  ----                                        │
 │      < >   Ceph core library                                         │
 │      < >   NFC subsystem support  ----                               │
 │      < >   Packet-sampling netlink channel  ----                     │
 │      < >   Inter-FE based on IETF ForCES InterFE LFB  ----           │
 │      [*]   Network light weight tunnels                              │
 │      [*]     Execute BPF program as route nexthop action             │
 │      <M>   Network physical/parent device Netlink interface          │
 │      < >   Generic failover module                                   │
        
                              │
┌── Networking options ────────────────────────────────────────────────┐
 │                                                                      │
 │ <*> Packet socket                                                    │
 │ < >   Packet: sockets monitoring interface                           │
 │ <*> Unix domain sockets                                              │
 │ < >   UNIX: socket monitoring interface                              │
 │ < > Transport Layer Security support                                 │
 │ < > Transformation user configuration interface                      │
 │ < > Transformation virtual interface                                 │
 │ [*] Transformation sub policy support                                │
 │ [*] Transformation migrate database                                  │
 │ [ ] Transformation statistics                                        │
 │ < > PF_KEY sockets                                                   │
 │ [*] XDP sockets                                                      │
 │ [*] TCP/IP networking                                                │
 │ [*]   IP: multicasting                                               │
 │ [*]   IP: advanced router                                            │
 │ [*]     FIB TRIE statistics                                          │
 │ [*]     IP: policy routing                                           │
 │ [*]     IP: equal cost multipath                                     │
 │ [*]     IP: verbose route monitoring                                 │
 │ [ ]   IP: kernel level autoconfiguration                             │
 │ < >   IP: tunneling                                                  │
 │ < >   IP: GRE demultiplexer                                          │
 │ [*]   IP: multicast routing                                          │
 │ [*]     IP: multicast policy routing                                 │
 │ [*]     IP: PIM-SM version 1 support                                 │
 │ [*]     IP: PIM-SM version 2 support                                 │
│ [*]   IP: TCP syncookie support                                      │
 │ < >   IP: Foo (IP protocols) over UDP                                │
 │ < >   IP: AH transformation                                          │
 │ < >   IP: ESP transformation                                         │
 │ < >   IP: IPComp transformation                                      │
 │ < >   IP: IPsec transport mode                                       │
 │ < >   IP: IPsec tunnel mode                                          │
 │ < >   IP: IPsec BEET mode                                            │
 │ < >   INET: socket monitoring interface                              │
 │ [*]   TCP: advanced congestion control  --->                         │
 │ [*]   TCP: MD5 Signature Option support (RFC2385)                    │
 │ <*>   The IPv6 protocol  --->                                        │
 │ [ ]   NetLabel subsystem support                                     │
 │ -*- Security Marking                                                 │
 │ [ ] Timestamping in PHY devices                                      │
 │ [*] Network packet filtering framework (Netfilter)  --->             │
 │ [ ] BPF based packet filtering framework (BPFILTER)  ----            │
 │ < > The DCCP Protocol  ----                                          │
 │ < > The SCTP Protocol  ----                                          │
 │ < > The Reliable Datagram Sockets Protocol                           │
 │ < > The TIPC Protocol  ----                                          │
 │ < > Asynchronous Transfer Mode (ATM)                                 │
 │ < > Layer Two Tunneling Protocol (L2TP)  ----                        │
 │ < > 802.1d Ethernet Bridging                                         │
 │ < > Distributed Switch Architecture                                  │
 │ < > 802.1Q/802.1ad VLAN Support                                      │
 │ < > DECnet Support                                                   │
 │ < > ANSI/IEEE 802.2 LLC type 2 Support                               │
 │ < > Appletalk protocol support                                       │
 │ < > CCITT X.25 Packet Layer                                          │
 │ < > LAPB Data Link Driver                                            │
 │ < > Phonet protocols family                                          │
 │ < > 6LoWPAN Support  ----                                            │
 │ < > IEEE Std 802.15.4 Low-Rate Wireless Personal Area Networks su    │
 │ [*] QoS and/or fair queueing  --->                                   │
 │ [*] Data Center Bridging support                                     │
 │ < > DNS Resolver support                                             │
 │ < > B.A.T.M.A.N. Advanced Meshing Protocol                           │
 │ < > Open vSwitch                                                     │
 │ < > Virtual Socket protocol                                          │
 │ < > NETLINK: socket monitoring interface                             │
 │ [*] MultiProtocol Label Switching  --->                              │
│ < > Network Service Header (NSH) protocol  ----                      │
 │ < > High-availability Seamless Redundancy (HSR)                      │
 │ [ ] Switch (and switch-ish) device support                           │
 │ [*] L3 Master device support                                         │
 │ [ ] NCSI interface support                                           │
 │ [*] Network priority cgroup                                          │
 │ [*] Network classid cgroup                                           │
 │ [*] enable BPF Just In Time compiler                                 │
 │ [*] enable BPF STREAM_PARSER                                         │
 │     Network testing  --->   
                                         │
 ┌── Network packet filtering framework (Netfilter) ────────────────────┐
 │                                                                      │
 │                                                                  │
 │        --- Network packet filtering framework (Netfilter)            │
 │        [*]   Advanced netfilter configuration                        │
 │              Core Netfilter Configuration  --->                      │
 │        < >   IP set support  ----                                    │
 │        < >   IP virtual server support  ----                         │
 │              IP: Netfilter Configuration  --->                       │




┌── Core Netfilter Configuration ──────────────────────────────────────┐
 │                                                                      │
 │    [*] Netfilter ingress support                                     │
 │    < > Netfilter NFACCT over NFNETLINK interface                     │
 │    < > Netfilter NFQUEUE over NFNETLINK interface                    │
 │    < > Netfilter LOG over NFNETLINK interface                        │
 │    < > Netfilter OSF over NFNETLINK interface                        │
 │    < > Netfilter connection tracking support                         │
 │    < > Netdev packet logging                                         │
 │    <M> Netfilter nf_tables support                                   │
 │    < >   Netfilter nf_tables set infrastructure                      │
 │    [*]   Netfilter nf_tables netdev tables support                   │
 │    < >   Netfilter nf_tables number generator module                 │
 │    < >   Netfilter nf_tables counter module                          │
 │    < >   Netfilter nf_tables log module                              │
 │    < >   Netfilter nf_tables limit module                            │
 │    < >   Netfilter nf_tables tunnel module                           │
 │    < >   Netfilter nf_tables stateful object reference module        │
 │    < >   Netfilter nf_tables quota module                            │
 │    < >   Netfilter nf_tables reject support                          │
 │    < >   Netfilter x_tables over nf_tables module                    │
 │    < >   Netfilter nf_tables hash module                             │
 │    < >   Netfilter nf_tables socket match support                    │
 │    < >   Netfilter nf_tables passive OS fingerprint support          │
 │    < >   Netfilter nf_tables tproxy support                          │
 │    < >   Netfilter packet duplication support                        │
 │    < >   Netfilter nf_tables netdev packet duplication support       │
 │    < >   Netfilter nf_tables netdev packet forwarding support        │


│   ┌── IP: Netfilter Configuration ───────────────────────────────────────┐
                                                                    │
 │  < > IPv4 socket lookup support                                      │
 │  < > IPv4 tproxy support                                             │
 │  [*] IPv4 nf_tables support                                          │
 │  < >   IPv4 nf_tables route chain support                            │
 │  < >   IPv4 nf_tables packet duplication support                     │
 │  < >   nf_tables fib / ip route lookup support                       │
 │  [*] ARP nf_tables support                                           │
 │  < > Netfilter IPv4 packet duplication to alternate destination      │
 │  < > ARP packet logging                                              │
 │  < > IPv4 packet logging                                             │
 │  < > IPv4 packet rejection                                           │
 │  <M> IP tables support (required for filtering/masq/NAT)             │
 │  < >   "ah" match support                                            │
 │  < >   "ecn" match support                                           │
 │  < >   "ttl" match support                                           │
 │  < >   Packet filtering                                              │
 │  < >   Packet mangling                                               │
 │  < >   raw table support (required for NOTRACK/TRACE)                │
 │  < >   Security table                                                │
 │  < > ARP tables support                                              │












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

