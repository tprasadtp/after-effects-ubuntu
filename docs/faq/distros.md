# What all distributions are supported?

In short? Ubuntu, its official flavors (Kubuntu,Ubuntu Mate etc), Linux Mint and Elementary.

??? info "About 32 bit Support"
    - Though 32 bit is supported, Testing in Travis CI, containers and locally all are done using 64 bit machine and containers. If something breaks please report it and use it with caution on 32 bit machines.
    - Since 17.10 Ubuntu no longer provides 32 bit ISO images. You have to use Ubuntu flavors like Lubuntu. Xubuntu or use minimal ISO.

!!! warning "Warning!"
    **Script will exit, if it cannot recognize the distribution.**

A Comple te list of supported distributions is given below.

Distribution     | Codename/Version  |   Supported | Notes
:----------------|:------------------|-------------|:------
Ubuntu 18.04     | Bionic Beaver     | Yes         |
Ubuntu 17.10     | Artful Aardvark   | Yes         |
Ubuntu 16.04     | Xenial Xerus      | Yes         |
Ubuntu 14.04     | Trusty Thar       | Yes         |
Ubuntu 18.10     | Cosmic Cuttlefish | No          | Only use it for testing
Linux Mint 17    | Quina             | Yes         |
Linux-Mint 17.1  | Rebecca           | Yes         |
Linux-Mint 17.2  | Rafaela           | Yes         |
Linux-Mint 17.3  | Rosa              | Yes         |
Linux Mint 18    | Sarah             | Yes         |
Linux-Mint 18.1  | Serena            | Yes         |
Linux-Mint 18.2  | Sonya             | Yes         |
Linux-Mint 18.3  | Sylvia            | Yes         |
Linux Mint 19    | Tara              | No          | Will be in the future
Elementary-OS    | Freya             | Yes         |
Elementary-OS    | Loki              | Yes         |
Budgie Remix     | 16.04             | Yes         |
PoP! OS          | 17.10 & 18.04     | Yes         |
Linux-Lite       | 3.X               | Yes         | (Based on Ubuntu 16.04)
Zorin-OS         | 12.X              | Yes         | (Based on Ubuntu 16.04)
Bodhi Linux      | 4                 | Yes         | (Based on Ubuntu 16.04)


??? info "Pre-Release and development builds"
    - Support for Ubuntu Pre-release builds, Elementary OS Juno are **experimental** and things might break.
    - They have not been released in stable release channels and are considered development versions of the release.
    - It is strongly advised to use them in a chroot or a in a VM and **not** as a daily driver.

??? info "New App-store on Linux Mint 18.3 and above"
    Linux mint 18.3 & later releases uses a new App-Store, from which you can directly install Chrome and other popular tools. There may be some conflicts in the `/etc/apt/sources.list.d`. Where, a single repository might be configured multiple times with same priority. Use it with caution. The scripts are not tested on Travis on Linux Mint.
