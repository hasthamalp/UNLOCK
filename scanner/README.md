# 8. Scanner

## How to install XSANE in Ubuntu

```
sudo apt install xsane
```

**You must install the mono package to complete the scanner installation**

{% tabs %}
{% tab title="Ubuntu 20.04" %}
```
sudo apt install gnupg ca-certificates
```

```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
```

```
echo "deb https://download.mono-project.com/repo/ubuntu stable-focal main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list
```

```
sudo apt update
```


{% endtab %}

{% tab title="Ubuntu 18.04" %}
```
sudo apt install gnupg ca-certificates
```

```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
```

```
echo "deb https://download.mono-project.com/repo/ubuntu stable-bionic main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list
```

```
sudo apt update
```


{% endtab %}

{% tab title="Ubunt 16.04" %}
```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF

```

```
sudo apt install apt-transport-https ca-certificates
```

```
echo "deb https://download.mono-project.com/repo/ubuntu stable-xenial main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list

```

```
sudo apt update
```
{% endtab %}
{% endtabs %}

Once the apt repository is enabled , update the packages list and install Mono with:

```
sudo apt update
```

```
sudo apt install mono-complete
```

Verify the installation by typing the following command which will print the Mono version:

```
mono --version
```



> ## Identify which scanner is used

```
scanimage -L
```



## TO detect all USB's

```
lsusb
```

## What to do in a situation where a simple scan does not open

Go to `Home`---->`.Cache`(view hidden files)------>`Simple-scan`

{% hint style="success" %}
Delete the `simple scan` folder.This will clear the cache in that software and This will help to open the simple scan properly .


{% endhint %}

## Installation of CANON PIXMA GM4070

Step1: Download and install [<mark style="color:blue;">IJ Printer Driver</mark>](https://in.canon/en/support/0101073801?model=3111C)

Step 2: Download and install [<mark style="color:blue;">ScanGear</mark>](https://in.canon/en/support/0101074101?model=3111C)

Step 3: Run the following command to add the PPA.

{% code fullWidth="true" %}
```bash
sudo add-apt-repository ppa:thierry-f/fork-michael-gruz
```
{% endcode %}

Step 4: Run the following command to install ScanGear MP in Ubuntu

```
sudo apt install scangearmp2
```

## KODAK i2620 Scanner

[i2620 Scanner|Ubuntu 16.04 LTS-32bit](https://resources.kodakalaris.com/docimaging/drivers/LinuxSoftware\_i2000\_v4.14.i586.deb.tar.gz)

[i2620 Scanner| Ubuntu - 64 bit](https://resources.kodakalaris.com/docimaging/drivers/LinuxSoftware\_i2000\_v4.14.x86\_64.deb.tar.gz)

**Expand the file (e.g., tar -xf \*.gz) and then run the setup script (i.e. sudo ./setup)**

[i2620 Scanner| Ubuntu 18.04 LTS](https://resources.kodakalaris.com/docimaging/drivers/LinuxSoftware\_i2000\_v4.14.x86\_64.deb.tar.gz)&#x20;

the following command must be entered in a terminal window:

```
sudo ln -sfr /usr/lib/sane/libsane-kds* /usr/lib/x86_64-linux-gnu/sane
```

