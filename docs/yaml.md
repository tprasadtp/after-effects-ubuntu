## YAML Config

The configuration file is pretty much self explanatory so, I am going to just post a sample config file below. All boolean fields are optional and if not provided or if found to be invalid, fallback to false.

```yml
# Install Config
version: 3
name: Polaris
author: Prasad T
# Configuraion
config:
  # Enabled Tasks
  tasks:
    update: true
    upgrade: true
    # Add Repos
    # individual repos flags are mentioned under config.add_repo key
    repo: true
    # Add PPAs
    ppa: true
    # APT Packages
    apt: true
    # Whether to purge packages mentioned in config.purge key
    purge: true
    debs: true
    pip2: true
    pip3: true

  # Repository Flags
  add_repo:
    winehq: true
    docker: true
    mendeley: false
    googlecloud: true
    spotify: true
    vscode: true
    skype: true
    signal: false
    insync: true
    google: true
    kubernetes: false
  # Flags
  flags:
  # Simulate flag will never be overridden by remote config.
    purge_enabled: true
    preserve_debs: true
    auto_yes: true

  # Packages to purge
  purge:
    - gnome-mines
    - gnome-sudoku
    - aisleriot
    - gnome-mahjongg
  # PPA List
  ppa:
    - ppa:dawidd0811/neofetch
    - ppa:yubico/stable
    - ppa:teejee2008/ppa
  # Install components
  # APT Packages, Python Modules, Debian packages
  install:
    # Python 2 Modules
    python2:
      - docker-compose
    # Python 3 Modules
    python3:
      - awscli
    # Debian packages:  .deb files
    # CSV format similar to lists
    debian_packages:
      - https://atom-installer.github.com/v1.28.0/atom-amd64.deb,Atom-Editor.deb
      - https://download.teamviewer.com/download/teamviewer_i386.deb,Teamviewer.deb
    apt:
      # Admin related Stuff
      administration:
        - dconf-editor
        - htop
        - apt-xapian-index
        - gdebi
        - gparted
        - synaptic
        - bleachbit
        - nautilus-admin
      # Security Related Stuff
      security:
        - gufw
      # Productiviy & Office Tools & Writing Tools
      productivity:
        - empathy
        - evolution
        - polari
        - realmd
        - pandoc-data
        - pandoc
        - texstudio
        - texlive-fonts-extra
        - texlive-formats-extra
        - texlive-fonts-recommended
        - texlive-science
        - texlive-generic-extra
        - texlive-xetex
        - texlive-luatex
        - texlive-pstricks
        - texlive-science
        - texlive-extra-utils
        - texlive-lang-english
        - texlive-lang-other
        - texlive-font-utils
        - texlive-publishers
        - gummi
      # Multimedia Tools. Photo Editots Converting tools, plex etc.
      multimedia:
        - audacity
        - vlc
        - gimp
        - handbrake
        - handbrake-cli
        - rawtherapee
        - darktable
        - mpv
        - pavucontrol
        - cheese
      # Tools related to development.
      development:
        - curl
        - spyder
        - spyder3
        - git
        - shellcheck
        - ocl-icd-dev
        - opencl-headers
        - clinfo
        - vainfo
        - vdpauinfo
        - ocl-icd-libopencl1
        - ruby
        - ruby-dev
        - python-magic
        - putty
        - s3cmd
        - python3-pip
        - python-dateutil
        - python-pip-whl
        - python-pip
      # Everything Else
      # Which is conditional
      other:
        - mesa-opencl-icd
        - opencl-clhpp-headers
        - opencl-c-headers
        - arc-theme
        - icedtea-8-plugin
        - openjdk-8-jre
        - neofetch
        - gnome-online-miners
        - telepathy-accounts-signon
        - signon-ui-service
      # Packages supplied by external repositories & PPAs
      # Dont Mix packages provided by distribution and PPAs
      # Sometimes external repos and ppas fail, so better isolate it.
      external:
        - google-chrome-stable
        - spotify-client
        - code
        - google-cloud-sdk
        - gcsfuse
        - docker-ce

```