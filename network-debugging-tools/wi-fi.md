# Wi-Fi

{% hint style="warning" %}
 **Wifi Network not appearing in Ubuntu \[HP\]**
{% endhint %}

![](../.gitbook/assets/15178-women-no-internet-wifi-off-data-off%20%281%29.gif)

Solution

```text
sudo apt-get install bcmwl-kernel-source 
```

##  Fix no WiFi in Ubuntu with broadcom wireless adapters

{% hint style="info" %}
This method is exclusively for Broadcom 43 series of wireless adapters. So make sure that you have these adapters by using this command:
{% endhint %}

```text
sudo lshw -C network
```

![](../.gitbook/assets/20210705_162317.jpg)

{% hint style="info" %}
If you see a wireless network adapter starting with BCM43, then only you should go ahead .
{% endhint %}

```text
sudo apt remove broadcom-sta-dkms bcmwl-kernel-source
```

```text
sudo apt install firmware-b43-installer
```

{% hint style="info" %}
Once the install is finished doing its work, you’ll need to reboot. After you log back in, you’ll be able to see and access your wifi connections. ✅ 
{% endhint %}

