# 7. Printer

![](../.gitbook/assets/753-printer.gif)

##

## Identify installed printers in  system

```
lpstat -a
```

## **How do I remove hundreds of automatically added network printers**

```
sudo nautilus
```

> 1.Go to `etc`-->`cups-->cups-browsed.conf`

&#x20;2.Change this line: `BrowseRemoteProtocols dnssd cups` (or whaterver is after   it) to none so it reads: `BrowseRemoteProtocols none`



> 3.stop cups and then remove the printers from the file

```
sudo service cups-browsed stop
```

## ADDING A NETWORK PRINTER (UBUNTU)

> &#x20;1.`System Settings --> Printers`
>
> 2\. Click `Add` and select `Find Network Printer`
>
> 3\. Enter the `IP address` in the `Host` field, and click `Find.`
>
> 4\. Click `Forward` and wait while the system searches for drivers
>
> 5\. Click `Apply` to finish

## &#x20;HPLIP Driver Installation Process

> **my HP printer supported by HPLIP please\[** [**check here**](https://developers.hp.com/hp-linux-imaging-and-printing/supported\_devices/index?language=es)**]**

1.First, download the latest **HPLIP(HP Linux Imaging and Printing)** driver from [\[website\]](https://developers.hp.com/hp-linux-imaging-and-printing/gethplip)

2.Secondly: after downloading the file it needs to be made executable. To do this, the following needs to be done:



* Open a terminal
* Browse to the Downloads folder: **`cd Downloads`**
* Then type the following command: **`sudo chmod +x hplip-*.**.**.run`**(\*.\*\*.\*\* is where the version number of the file needs to be filed in)\
  ****
* Press Enter and if required, type the _ **user password** _ and press Enter

The HPLIP driver is now executable. Keep the terminal open.

{% hint style="danger" %}
&#x20;Do not switch on the printer during the installation procedure!!! If the printer is switched on, make sure it is switched off before starting the installation procedure.\

{% endhint %}

To run the installation file it is not required to use `sudo` to get root privileges. In the terminal type the following command: **`./hplip-.*..run`**

{% hint style="info" %}
:man\_detective: Note that the command **starts with . (dot) / (slash)** followed by the complete filename and **ending on . (dot) run!**
{% endhint %}

before the installation procedure starts the user must choose whether to install the driver **manually** (press **c** for **custom**) or **automatically** (press **a** for **automatic**). Best is to execute the installation procedure manually (custom) so that every step can be controlled and monitored by the user.

The installation procedure will check for missing ask if older versions of the HPLIP driver must be removed. Confirm that this should be done to avoid any conflicts with older package versions.

![](../.gitbook/assets/20210524\_104027.jpg)

{% hint style="info" %}
:woman\_guard: Always restart the computer, re-plugging in the printer doesn't always work. By restarting the computer and after logging in switching on the printer, the user forces Ubuntu to search for any printers connected.
{% endhint %}

![](../.gitbook/assets/printer.jpg)

> :white\_check\_mark: HPLIP Driver installed Successfully

## Is HPLIP currently installed?

**Debian package based distributions (Debian, Ubuntu, Mepis, etc):**

Run in a terminal window:

```
dpkg -l hplip
```

You may see something that looks like this:

![](../.gitbook/assets/hplip.JPG)

{% hint style="info" %}
If you see "ii" in the first column before "hplip", then HPLIP is already installed. If you want to use the currently installed version of HPLIP, try running `hp-setup` in a terminal shell.
{% endhint %}

Try below method for <mark style="background-color:green;">HP Scanner plugin issues</mark>. first install HPLIP latest version on system and try following steps.

Download Latest [Plugins](https://developers.hp.com/hp-linux-imaging-and-printing/plugins) from HP website: version may vary

Run this command to Install Plugin:

```
sh hplip-3.21.12-plugin.run
```

{% hint style="success" %}
That fixed the Scanner issue.Now you able to scan without any issues.:smile:
{% endhint %}

{% embed url="https://openprinting.org/printers" %}
