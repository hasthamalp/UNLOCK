# Wi-Fi

{% hint style="warning" %}
 **Wifi Network not appearing in Ubuntu \[HP\]**
{% endhint %}

![](../.gitbook/assets/15178-women-no-internet-wifi-off-data-off%20%281%29.gif)

Solution

```text
sudo apt-get install bcmwl-kernel-source 
```

## WiFi not working in HP laptop RTL8723DE Realtek wireless driver

{% hint style="info" %}
This method is exclusively for RTL8723DE series of wireless adapters. So make sure that you have these adapters by using this command:
{% endhint %}

```text
sudo lshw -C network
```

{% hint style="info" %}
If you see a wireless network adapter starting with RTL, then only you should go ahead
{% endhint %}

```text
sudo apt update
```

```text
sudo apt install git dkms
```

```text
git clone https://github.com/smlinux/rtl8723de.git -b 4.11-up
```

```text
sudo dkms add ./rtl8723de
```

```text
sudo dkms install rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414
```

```text
sudo depmod -a
```

✅ Reboot 📶 and your wireless should be working. 😀 

##  Fix no WiFi in Ubuntu with **Broadcom** wireless adapters

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

