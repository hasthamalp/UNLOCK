---
description: Ubuntu Quick Setup Follow these simple steps to start using Flatpak
---

# Malayalam editor\(Varnam Editor\)

### 1.Install Flatpak

> To install Flatpak on Ubuntu 18.10 \(Cosmic Cuttlefish\) or later, simply run:

```text
sudo apt install flatpak
```

> With older Ubuntu versions, the official Flatpak PPA is the recommended way to install Flatpak. To install it, run the following in a terminal:

```text
sudo add-apt-repository ppa:alexlarsson/flatpak
sudo apt update
sudo apt install flatpak
```

## 2 Install the Software Flatpak plugin

> The Flatpak plugin for the Software app makes it possible to install apps without needing the command line. To install, run:

```text
sudo apt install gnome-software-plugin-flatpak
```

{% hint style="info" %}
👮 Note: the Software app is distributed as a Snap since Ubuntu 20.04 and does not support graphical installation of Flatpak apps. Installing the Flatpak plugin will also install a deb version of Software and result in two Software apps being installed at the same time.
{% endhint %}





## 3 Add the Flathub repository

> Flathub is the best place to get Flatpak apps. To enable it, run:

```text
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

## 4. Restart

> To complete setup, restart your system. install [Malayalam editor\(Varnam Editor\)](malayalam-editor.md#varnam-editor-installation)



### 

### 

### Varnam Editor Installation

> Varnam helps you to type Indian languages like Malayalam, Hindi, Tamil, Telugu, Bangla with english letters. It transliterates english text to the corresponding Indian language

> **Install:**

> Make sure to follow the [setup guide](https://flatpak.org/setup/Ubuntu/) before installing

```text
flatpak install flathub com.varnamproject.Varnam
```

> **Run:**

```text
flatpak run com.varnamproject.Varnam
```

