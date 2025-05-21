---
icon: share
---

# SHARE

## Install Share on Ubuntu system

```
sudo apt-get install nfs-common
```

```
sudo apt-get -f install   
```

## create a directory called _share_

```
mkdir share
```

```
sudo nautilus  
```

{% hint style="info" %}
`computer`->`etc`->`fstab`->`10.69.51.20:`//share (tab)/`home`/`(computername)`/`share` (tab) `nfs` (tab) defaults (tab) `0` (tab) `0`->`save`.**(NB:IP Address different for different district)**
{% endhint %}

```
sudo mount -a   
```

{% hint style="success" %}
SHARE  is now done successfully on your system
{% endhint %}
