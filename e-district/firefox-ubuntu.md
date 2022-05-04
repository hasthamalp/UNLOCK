# Firefox Ubuntu

<mark style="background-color:purple;">**The  eDistrict  Version 2.0 is**</mark><mark style="background-color:purple;">** **</mark>_<mark style="background-color:purple;">**not dependent on Java applet and will work with Latest version of Firefox**</mark>_<mark style="background-color:purple;">** **</mark><mark style="background-color:purple;">**and as well as google chrome**</mark>_<mark style="background-color:purple;">**.**</mark>_

![](https://www.mozilla.org/media/img/firefox/template/page-image-master.1b6efe3d5631.jpg)

_The latest Firefox  version  is_ <mark style="background-color:green;">**99**</mark>

## Firefox Installation

1. Download Firefox
2. Extract the contents of the downloaded file by typing:

```
tar xjf firefox-*.tar.bz2
```

3\. Move the uncompressed Firefox folder to /opt:

```
mv firefox /opt
```

4\. Create a symlink to the Firefox executable:

```
ln -s /opt/firefox/firefox /usr/local/bin/firefox
```

5\. Download a copy of the desktop file:

```
wget https://raw.githubusercontent.com/mozilla/sumo-kb/main/install-firefox-linux/firefox.desktop -P /usr/local/share/applications
```

{% hint style="success" %}
Latest Version Firefox Installed on your system Successfully.
{% endhint %}

## Upgrade Firefox on Ubuntu

```
sudo apt-get update
```

```
sudo apt-get install --only-upgrade firefox
```

## Uninstall firefox on Ubuntu

```
sudo apt-get purge firefox
```
