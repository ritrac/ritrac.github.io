---
title: BabelZone
description: iozone on various devices
subtitle: iozone on various devices
tags:
    - iozone
---

## Benchmark

* Unmodified **[IOzone](https://www.iozone.org/)** in auto mode
* Figures generated with Python/Pandas/Matplotlib
* Free memory: ~3GB (-> buffer cache smaller than 3GB)
    * smaller runtime

!!! warning
    Don't forget the buffer cache behavior !


## Results

### HDD

#### Hitachi Ultrastar SATA 7200RPM

Datasheet:

* PN: HUA722010CLA330
* Disk Family: Ultrastar A7K2000
* Form Factor: 3.5"
* Capacity: 1TB
* Rotational Speed: 7200 RPM
* Rotation Time: 8.33ms
* Disk Interface: Serial-ATA/300
* Buffer-Host Max Rate: 300 MB/s
* Buffer Size: 32768 KB
* Weight: 680 grams
* Required Power For Spinup: 3300 mA
* Power Required (Seek | Idle | Standby): 7 W | 5 W | 2 W

![image](iozone-hdd-HUA722010CLA330-ext4-bw.svg)
![image](iozone-hdd-HUA722010CLA330-ext4-iops.svg)

### SSD sata

#### Crucial MX500 SATA

Datasheet:

* PN: CT1000MX500SSD1
* Memory Type: Micron 3D TLC NAND Flash
* Disk Family: MX500
* Form Factor: 2.5"
* Capacity: 1TB
* Disk Interface: Serial-ATA/600
* 512 byte sector size support
* Power Required (Seek | Sleep): 5 W | 3mW
* Endurance - total bytes written (TBW): Up to 1000TB

![image](iozone-sda-CT1000MX500SSD1-ext4-bw.svg)
![image](iozone-sda-CT1000MX500SSD1-ext4-iops.svg)

### SSD nvme

#### Samsung 970 Evo Plus 2TB

* Memory Type: Samsung V-NAND 3bit MLC
* PN: ???
* Cache Memory: 2GB LPDDR4
* Form Factor: M.2 (2280)
* Capacity: 2TB
* Disk Interface: PCIe Gen 3.0 x4 (x2 on the mother board)
* Power Required (Read | Write | Sleep): 5.5 W | 6 W | 5 mW
* Endurance - total bytes written (TBW): Up to 1200TB

![image](iozone-nvme-970evop-2TB-2x-bw.svg)
![image](iozone-nvme-970evop-2TB-2x-iops.svg)

!!! todo
    It should be nice to see the behavior of the LPDDR (cache ? buffer ?)

#### Samsung 970 Evo Plus 1TB 4X

!!! todo
    - Run IOzone
    - show the LPPDR too

### ZFS RAIDZ2

!!! Upcoming
    Coming soon :smile:

#### Mother Board Controller

#### HBA

### NFS


