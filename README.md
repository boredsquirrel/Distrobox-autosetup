# Distrobox-autosetup
Some scripts to automatically setup some Distroboxes like Arch with yay for using the AUR, Ubuntu with Nala, Fedora with RPMFusion and more.

Using Distrobox, a fork of Toolbox, you can run programs from many Distros containerized from your system. They work like regular apps, including GUI and a shared home folder. With `distrobox-export --app APPNAME` you can add the App to your Systems Applauncher as if it was native.
`
## Arch with AUR

1. Install the box

```
https://github.com/trytomakeyouprivate/Distrobox-autosetup/raw/main/Arch-with-yay
```

2. Setup yay

```
wget https://github.com/trytomakeyouprivate/Distrobox-autosetup/raw/main/Arch | bash
```

## Fedora

1. Install the box

```
distrobox create Fedora -i registry.fedoraproject.org/fedora-toolbox:37 && distrobox enter Fedora
```

2. Setup interactively

```
wget https://github.com/trytomakeyouprivate/Distrobox-autosetup/raw/main/Fedora | bash
```

## Ubuntu

1. Install the box

```
distrobox create Ubuntu -i docker.io/library/ubuntu:22.04 && distrobox enter Ubuntu
```

2. Setup nala, autoupdates and more

```
wget https://github.com/trytomakeyouprivate/Distrobox-autosetup/raw/main/Ubuntu | bash
```

3. Install some needed packages

```
sudo nala install software-properties-common
```

Android development example

```
sudo add-apt-repository ppa:maarten-fonville/android-studio
sudo nala install -y android-studio openjdk-8-jdk-headless
```
