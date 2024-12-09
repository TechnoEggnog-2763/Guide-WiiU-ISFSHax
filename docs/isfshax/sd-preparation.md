---
next: true
---

# SD Preparation

We will now put the required files for ISFSHax and DNSpresso on the SD Card.

::: warning

Your SD Card will need to be formatted as FAT32. If your SD Card is not formatted to FAT32, use [GUIFormat](http://ridgecrop.co.uk/index.htm?guiformat.htm) with 32k (32768) allocation unit size to format it.  
**Do not** label the SD Card as `wiiu` or it will cause issues with homebrew.

:::

## Instructions

1. Grab the the [ISFSHax Installer](https://github.com/isfshax/isfshax_installer/releases) (`ios.img`) and place it on the root of your SD Card.
2. Grab the contents of the [ISFSHax](https://github.com/isfshax/isfshax/releases) directory (`superblock.img` and `superblock.img.sha`) and place them on the root of your SD Card.
3. Create a new folder titled `wiiu`. In that folder, create another folder titled `ios_plugins`.
4. Grab the [stroopwafel](https://github.com/jan-hofmeier/stroopwafel/releases) (wafel_core.ipx), as well as the [ISFHax patch](https://github.com/isfshax/wafel_isfshax_patch/releases) and place them in the newly created `ios_plugins` folder.
5. Grab the [minute image](https://github.com/jan-hofmeier/minute_minute/releases) (`fw_encrypted`) and place it on the root of your SD Card. Rename it to `fw.img`.
6. Extract the [fw_img payload](https://github.com/wiiu-env/fw_img_payload/releases) and drag the `wiiu` folder to the root of your SD Card.
 - The `wiiu` folders should be merged if not done automatically.
7. Extract the [root.rpx](https://github.com/wiiu-env/PayloadFromRPX/releases) and place it on the root of your SD Card. Rename it to `launch.rpx`.

## SD Card Layout

::: details Click here to show the final SD Card layout.

```
💾sd:
 ┣ 📂wiiu
 ┃   ┣ 📂ios_plugins
 ┃   ┃  ┣ 📜wafel_core.ipx
 ┃   ┃  ┗ 📜wafel_isfshax_patch.ipx
 ┃   ┣ 📂payloads
 ┃   ┃  ┗ 📂fw_img loader
 ┃   ┃  ┃  ┗ 📜payload.elf
 ┣ 📜fw.img
 ┣ 📜ios.img
 ┣ 📜superblock.img
 ┣ 📜superblock.img.sha
 ┗ 📜launch.rpx
```

:::
