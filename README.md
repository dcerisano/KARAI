# ATARI IRATA

- A dev and deploy environment for Atari 8-bit made of popular components (Git, Altirra, AspeQT, bash, etc)
- Produces self booting Atari floppy images (bootable ATR files)
- A sample project (atariVT) to repurpose an 8K Atari 400 as a server monitor.
- Should run on ANY 8-bit Atari computer with minimum 8K RAM.
  
![dev](https://github.com/dcerisano/atariVT/assets/1641613/68212175-384d-4535-accc-874a3385c240)

https://github.com/dcerisano/atariVT/assets/1641613/5dabed1b-acfc-47c6-b7b9-8cb8448e9d7d

https://8bitworkshop.com/dithertron


- Uses AspectQT on the host with sio2usb connector (FTDI) to the 400 SIO (see diagram)
- Host acts as 810 floppy drive to boot the 400 (D1:/../ATR/ATARIVT.ATR)
- Server script (atarivt.sh) streams data frames to shared folder (D2:/../ATR)
- Used Atari800 (Altirra) for development with real 8K Atari 400 for testing.

- DONE: Page flipped data frame buffering (40x24 text frame)
- DONE: Animated GR.7 autorun.bas boot splash using DLI
- DONE: dithertron.sh for converting dithertron images to Atari-readable files
- TODO: Port BASH script to MSDOS batch file
- TODO: Animated LCARS graphics, of course.
