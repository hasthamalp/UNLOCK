---
icon: firefox-browser
---

# Firefox Ubuntu

<mark style="background-color:purple;">**The  eDistrict  Version 2.0 is not dependent on Java applet and will work with Latest version of Firefox and as well as google chrome.**</mark>

The latest Firefox  version  is <mark style="color:red;background-color:red;">144.0.0</mark>

![](https://www.mozilla.org/media/img/structured-data/logo-firefox-browser.fbc7ffbb50fd.png)

## Firefox Installation

<details>

<summary>Download Firefox</summary>

1.Extract the contents of the downloaded file by typing:

```
tar xjf firefox-*.tar.bz2
```

2.Move the uncompressed Firefox folder to /opt:

```
mv firefox /opt
```

3.Create a symlink to the Firefox executable:

```
ln -s /opt/firefox/firefox /usr/local/bin/firefox
```

4\. Download a copy of the desktop file:

```
wget https://raw.githubusercontent.com/mozilla/sumo-kb/main/install-firefox-linux/firefox.desktop -P /usr/local/share/applications
```

</details>

{% hint style="success" %}
Latest Version of Firefox Installed on your system Successfully.
{% endhint %}

## Update Firefox Ubuntu

```
sudo apt update
```

```
 sudo apt install --only-upgrade firefox
```
