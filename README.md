# alpineSetup
Instructions to setup alpine linux, specifiaclly on the HP Elitebook 850 G6

# Part A: Create a bootable USB and install the base system

1. Get the most recent alpine iso [here](https://alpinelinux.org/downloads/)
2. Flash it to an empty USB drive using something like gnome-disks or rufus
3. Boot to the newly flashed USB and run the `setup-alpine` command. This will start an interactive installation process
4. Most of the options will be self explanatory. When asked what type of disk mode to use, select `sys`. This will install alpine to the harddrive

# Part B: setting up the base system

TODO

# Part C: QoL and other nice stuff

## Anaconda

- Anaconda is linked into glibc, so you will have to install glibc. Instrcutions are available [here](https://github.com/sgerrand/alpine-pkg-glibc)

## Sound

- Enable detection of the sound card by adding `snd-intel-dspcfg.dsp_driver=1` to the kernel options

# Part D: Other stuff

- Blacklist the pcspkr module to prevent annoying beeping in TTY
