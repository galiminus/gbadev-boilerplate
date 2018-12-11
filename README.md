# Dependencies (ubuntu)

Install the pacman version of Devkitpro:

```
wget https://github.com/devkitPro/pacman/releases/download/devkitpro-pacman-1.0.1/devkitpro-pacman.deb
sudo dpkg -i devkitpro-pacman.deb
sudo dkp-pacman -S gba-dev
rm devkitpro-pacman.deb
```

DevkitPro packages should be install in `/opt/devkitPro`.

# Build

Use `make build` to generate `main.gba`.
Use `make run` to build and run with the MGBA emulator.

You can change both the DevkitPro location and emulator with environment variables.

```
EMULATOR=another_emulator DEVKITPRO=/usr/local/devkitpro make run`
```

Use `make clean` to clean up all temporary files.
