# Wi-Fi

{% hint style="warning" %}
 **Wifi Network not appearing in Ubuntu**
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

```text
sudo apt remove broadcom-sta-dkms bcmwl-kernel-source
```

{% hint style="info" %}
If you see a wireless network adapter starting with BCM43, then only you should go ahead .
{% endhint %}

```text
sudo apt install firmware-b43-installer
```

{% hint style="info" %}
Once the install is finished doing its work, you’ll need to reboot. After you log back in, you’ll be able to see and access your wifi connections. ✅ 
{% endhint %}

## Fix ‘No WiFi Adapter Found’ for HP Laptops with Ubuntu 18.04

```text
sudo apt-get install linux-headers-$(uname -r) build-essential git
```

```text
git clone https://github.com/lwfinger/rtlwifi_new.git
```

```text
cd rtlwifi_new/ && git checkout origin/extended -b extended
```

```text
sudo make install
```

```text
sudo modprobe -r rtl8723de
```

```text
sudo modprobe rtl8723de
```

```text
sudo apt purge bcmwl-kernel-source
```

```text
sudo sed -i '/blacklist bcma/ d' /etc/modprobe.d/blacklist.conf
```

```text
sudo sed -i '/blacklist brcmsmac/ d' /etc/modprobe.d/blacklist.conf
```

```text
sudo modprobe -r rtl8723de && sleep 5 && sudo modprobe rtl8723de ant_sel=1
```

```text
sudo modprobe -r rtl8723de && sleep 5 && sudo modprobe rtl8723de ant_sel=2
```

```text
echo "options rtl8723de ant_sel=X" | sudo tee /etc/modprobe.d/rtl8723de.conf
```

{% hint style="success" %}
success
{% endhint %}

