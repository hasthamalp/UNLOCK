# Wi-Fi

{% hint style="warning" %}
&#x20;**Wifi Network not appearing in Ubuntu \[HP]**
{% endhint %}

![](../.gitbook/assets/75267-no-wifi.gif)

Solution

```
sudo apt-get install bcmwl-kernel-source 
```

#### Command to check  network driver installed on your system

```
lspci | grep Network
```

## WiFi not working in HP laptop RTL8723DE Realtek wireless driver

{% hint style="info" %}
This method is exclusively for RTL8723DE series of wireless adapters. So make sure that you have these adapters by using this command:
{% endhint %}

```
sudo lshw -C network
```

{% hint style="info" %}
If you see a wireless network adapter starting with RTL, then only you should go ahead
{% endhint %}

```
sudo apt update
```

```
sudo apt install git dkms
```

```
git clone https://github.com/smlinux/rtl8723de.git -b 4.11-up
```

```
sudo dkms add ./rtl8723de
```

```
sudo dkms install rtl8723de/5.1.1.8_21285.20171026_COEX20170111-1414
```

```
sudo depmod -a
```

:white\_check\_mark: Reboot :signal\_strength: and your wireless should be working. :grinning:&#x20;

**OR TRY THIS**

&#x20;**recommend for HP users facing WiFi problem**

```
sudo apt-get install linux-headers-$(uname -r) build-essential git
```

```
git clone https://github.com/lwfinger/rtlwifi_new.git
```

```
cd rtlwifi_new/ && git checkout origin/extended -b extended
```

```
sudo make install
```

```
sudo modprobe -r rtl8723de
```

```
sudo modprobe rtl8723de
```

```
sudo apt purge bcmwl-kernel-source
```

```
sudo sed -i '/blacklist bcma/ d' /etc/modprobe.d/blacklist.conf
```

```
sudo sed -i '/blacklist brcmsmac/ d' /etc/modprobe.d/blacklist.conf
```

```
sudo modprobe -r rtl8723de && sleep 5 && sudo modprobe rtl8723de ant_sel=1
```

```
sudo modprobe -r rtl8723de && sleep 5 && sudo modprobe rtl8723de ant_sel=2
```

```
echo "options rtl8723de ant_sel=X" | sudo tee /etc/modprobe.d/rtl8723de.conf
```

:signal\_strength: Reboot your PC.

## &#x20;Fix no WiFi in Ubuntu with **Broadcom** wireless adapters

{% hint style="info" %}
This method is exclusively for Broadcom 43 series of wireless adapters. So make sure that you have these adapters by using this command:
{% endhint %}

```
sudo lshw -C network
```

![](../.gitbook/assets/20210705_162317.jpg)

{% hint style="info" %}
If you see a wireless network adapter starting with BCM43, then only you should go ahead .
{% endhint %}

```
sudo apt remove broadcom-sta-dkms bcmwl-kernel-source
```

```
sudo apt install firmware-b43-installer
```

{% hint style="info" %}
Once the install is finished doing its work, you’ll need to reboot. After you log back in, you’ll be able to see and access your wifi connections. :white\_check\_mark:&#x20;
{% endhint %}

## Ubuntu WiFi is disabled

![](../.gitbook/assets/wifiissue.jpg)

{% hint style="info" %}
Simply putting it on `suspend` and bringing it back up seems to make the wifi work normally.**This is not a permanent solution.**&#x54;he only problem is to do this every time  start Ubuntu.
{% endhint %}

just want to reactivate your WiFi

**rfkill** command used to `enable/disable` network drivers or activate or deactivate Network Adapters

```
sudo rfkill unblock wifi
```
