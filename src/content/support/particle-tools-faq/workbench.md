---
title: Workbench
layout: support.hbs
columns: two
order: 900
---

# Particle Workbench FAQ

{{!-- FAQs: See ch25557 --}}

- [Installation Instructions](/quickstart/workbench/)
- [Tutorial](/tutorials/developer-tools/workbench)

## Working with a custom Device OS build

It's possible to work with a non-released branch, fork, or manually merged PRs of Device OS.

- Get the latest Device OS source from GitHub. You'll need to have the command line version of git available in order to retrieve the submodules.

```
git clone git@github.com:particle-iot/device-os.git
cd ./device-os
git submodule update --init --recursive
git checkout -b develop
```

- Run the `Particle: Launch Compiler Shell` command.
- In the terminal that launches, execute the following:

```
DEVICE_OS_PATH=/path/to/device-os/ make -f $PARTICLE_MAKEFILE compile-all
```

- You'll need to do your builds from this window in order for the change to take effect.


## Uninstalling Workbench

- Open VSCode.
- Click the **Extensions** button on the left toolbar (Activity bar).
- Click on the gear icon for the **Workbench** extension and select **Uninstall**.
- Repeat for the **C/C++** and **Cortex-Debug** extensions
- Close and re-open VSCode, then close it again.
- Delete the `~/.particle/toolchains` directory.

## Uninstalling VSCode

### Mac

- Find your `Visual Studio Code.app` file (typically in `~/Applications` or `/Applications`)
- Delete `Visual Studio Code.app`

### Windows 

- Open **Add/Remove Programs**.
- Select **Microsoft Visual Studio Code** and click the **Uninstall** button

### Linux 

- Open a terminal
- Run `sudo apt-get purge code`. This currently only works with Ubuntu and other Debian-style distributions.

## Linux Tips

- On 64-bit Linux you may need to install 32-bit libraries:

```
sudo apt-get install gcc-multilib libncurses5:i386
```

- If you get a permission error when debugging, you may need to add udev rules.
  * If you have the [Particle Workbench](https://docs.particle.io/workbench/), run the `Particle: Launch CLI` command and then run `particle usb configure` in the terminal that launches
  * if you just have the [Particle CLI](https://docs.particle.io/tutorials/developer-tools/cli/), open a terminal and run `particle usb configure`
  * Otherwise, you can download [50-particle.rules](https://github.com/particle-iot/particle-cli/blob/master/assets/50-particle.rules) and copy it to `/etc/udev/rules.d/`



