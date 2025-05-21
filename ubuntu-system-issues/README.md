---
icon: spoon
---

# 5. Issues and Solutions

![](<../.gitbook/assets/Bug fixing.gif>)

{% hint style="danger" %}
**1**.Initramfs Issue BusyBox /fsck error
{% endhint %}

![](../.gitbook/assets/FSCK.jpg)

> solution

```
fsck /dev/sdaX
```

&#x20;`/dev/sda1` is the first partition of first drive. X- partition

```
reboot
```

If you don't want to manually press 'y' every time it asks for a fix, you can also run the command with the `-y` option.

```
fsck /dev/sdaX -y
```

{% hint style="info" %}
Error that occurred due to improper shutdown or Partial upgrades(**fsck**-**F**ile**S**ystem **C**hec**k)**
{% endhint %}

{% hint style="danger" %}
**2**.failed to start nvidia persistence daemon
{% endhint %}

![](../.gitbook/assets/500089300355_338398.jpg)

solution: first restart your system. then select `ubuntu` from GRUB menu. then press the `E` key. Add `nouveau.modeset=0` to the end of the `linux` line - press `F10` to boot.

{% hint style="info" %}
&#x20;`nomodeset` is a temporary solution in case a system does not boot without a proprietary driver. This is not to be used permanently.
{% endhint %}

{% hint style="danger" %}
**3**.Date and Time setting
{% endhint %}

> Solution

![](../.gitbook/assets/IMAGE2.jpg)

```
sudo date 010224311971.59
```

> OR

```
sudo date --set="2020-01-02 23:31:5
```

{% hint style="danger" %}
**4.GRUB RESCUE ISSUE**
{% endhint %}

![](../.gitbook/assets/grubpic.jpg)

> **solution:1**
>
> `grub>`**`set`**
>
> for Example:
>
> `root=hd0,msd0s7(output of`` `**`set`**`)this may change`
>
> `................................................`
>
> `grub rescue>set boot=(hd0,msd0s7)`
>
> `grub rescue>set prefix=(hd0,msd0s7)/boot/grub`
>
> `grub rescue>insmod normal`
>
> `grub rescue>normal`
>
> #### `Then login to ubuntu update Grub`
>
> &#x20;

```
sudo update-grub
```

```
sudo grub-install /dev/sda
```

**METHOD 1:**

![](../.gitbook/assets/grub.JPG)

**2**

![](../.gitbook/assets/grub2.JPG)

**3**

![](../.gitbook/assets/grub3.JPG)

OTHER LINKS:[<mark style="color:orange;background-color:purple;">GRUB RESCUE</mark>](https://www.pcsuggest.com/grub-rescue-linux/)<mark style="color:orange;background-color:purple;">1</mark>&#x20;

[<mark style="background-color:purple;">GRUB RESCUE LINK2</mark>](https://itsfoss.com/fix-minimal-bash-line-editing-supported-grub-error-linux/)



## How do I change the user account password?

```
passwd
```

## To change other users password:

```
sudo passwd USERNAME
```
