# MacBook Pro "Core i5" 2.4 13" Late 2011 	2.4 GHz Core i5 (I5-2435M)
	

|             |  |
| ----------- | ------------ |
| Intro.      | October 24, 2011 |
| Disc.       | June 11, 2012 |
| Serial      | C17H95S3DV13 |
| Order       | MD313LL/A |
| Model       | A1278 (EMC 2555*) |
| Family      | Late 2011 13"  |
| ID          | MacBookPro8,1    |
| RAM         | 4 GB |
| VRAM        | 384 MB |
| Storage     | 500 GB HDD 	Optical 	8X DL "SuperDrive" |

## To download

1. OpenCore Legacy Patcher 2.1.2 \
https://github.com/dortania/OpenCore-Legacy-Patcher/releases/tag/2.1.2
1. Monterey (final version) 12.7.6 \
https://mrmacintosh.com/macos-12-monterey-full-installer-database-download-directly-from-apple/
1. Ventura 13.7.2 \
https://mrmacintosh.com/macos-ventura-13-full-installer-database-download-directly-from-apple/
1. High Sierra 10.13.6 \
_From the App Store at the dad's laptop_

## Process

### SSD installation

A-OK.

#### Formatting
1. For _High Sierra_
    * Name: Macintosh SSD
    * Format: Mac OS Extended (case-sensitive, journaled); NON-encrypted
    * Scheme: GUID Partition Map
1. For _Monterey_
    * Format: APFS (case-sensitive)

Done.

### Followed tutorials

1. Create intial bootable installer: https://support.apple.com/en-us/101578
1. MrMacintosh step by step video tut: https://www.youtube.com/watch?v=-huRykhjs6g
1. Other guy's tut: https://www.youtube.com/watch?v=nn3jO8sxI8k
1. OCLP's docs: https://dortania.github.io/OpenCore-Legacy-Patcher/POST-INSTALL.html#booting-without-usb-drive, esp. to sort out the lack of pop-up to Build and Install OpenCore in the internal drive in order to settle down the installation.
