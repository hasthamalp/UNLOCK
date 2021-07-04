# Ubuntu Corner

![](../.gitbook/assets/ubuntu_plain_wordmark_logo_icon_146632.png)

{% hint style="info" %}
**Ubuntu X.YY**

**X-**representing the **year**

**YY** representing the **month of eventual release within in that year**

\*\*\*\*
{% endhint %}

{% hint style="info" %}
Ubuntu's first release, made in **2004 October \(10th month\)** was **Ubuntu 4.10**
{% endhint %}

{% hint style="info" %}
Software installation

* GNOME-Software
* Synaptic Package Manager
* GDebi Package Installer
* _apt -_Command Line Tool
{% endhint %}

## ഉബുണ്ടുവിൽ പാക്കേജുകൾ ഇൻസ്റ്റാൾ ചെയ്യുന്ന വിധം

```text
sudo apt install <package_name>
```

> Example:To install mplayer

**sudo apt install mplayer**



## **ഉബുണ്ടുവിൽ .deb പാക്കേജുകൾ ഇൻസ്റ്റാൾ ചെയ്യുന്ന വിധം**

\*\*\*\*

```text
sudo dpkg -i <file_name.deb>  
```

#### **Folder contain** _**sh**_ **file**

```text
 sudo ./install.sh
```

> OR

```text
 sudo sh install.sh               
```

**Folder contain `setup`file**

```text
sudo ./setup
```

## **ഉബുണ്ടുവിൽ പാക്കേജുകൾ Uninstall ചെയ്യുന്ന വിധം**

```text
 sudo apt remove <package_name>                         
```

> OR

```text
sudo apt purge <package_name>
```

**To see the details of a package**

```text
apt show <package_name>
```

## **The command to use as a super user on Ubuntu system**

```text
sudo nautilus
```

 **Guest Removal Ubuntu 16.04**

```text
 sudo mkdir /etc/lightdm/lightdm.conf.d
```



```text
 sudo sh -c 'printf "[SeatDefaults]\nallow-guest=false\n" > /etc/lightdm/lightdm.conf.d/50-no-guest.conf'
```

`restart system` 📶 

## Important apt Commands

| _apt_ Command | Function of the command |
| :--- | :--- |
| apt install | Installs a package |
| apt remove | Removes a package |
| apt purge | Removes package with configuration |
| apt update | Refreshes repository index |
| apt upgrade | Upgrade all upgradable packages |
| apt autoremove | Removes unwanted packages |
| apt search | Searches for the program |

## USEFUL LINUX COMMANDS 😁 

> **system information**

| **command** | Description |
| :--- | :--- |
| date | show the current date and time |
| uname -a |  show kernel information |
| cat /proc/cpuinfo |  cpu information |
| cat /proc/meminfo | memory information |
| man command | show the manual for command |

## UBUNTU SHORTCUTS 😎 

| Shortcut | Usage |
| :--- | :--- |
| Ctrl+C | halts the current command |
| Ctrl+Z | stops the current command |
| Ctrl+D | log out of current session, similar to exit |
| Ctrl+W | erases one word in the current line |
| Ctrl+U | erases the whole line |
| Ctrl+R |  type to bring up a recent command |
| !! | repeats the last command |
| exit | log out of current session |

## BOOT KEY

![](../.gitbook/assets/boot.jpg)

## BIOS KEY

![](../.gitbook/assets/bios.jpg)

\*\*\*\*

|  |
| :--- |
|  |

