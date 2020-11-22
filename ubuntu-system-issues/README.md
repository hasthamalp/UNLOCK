# Ubuntu System Issues

![](../.gitbook/assets/27659-bug-guy-1-.gif)

{% hint style="danger" %}
Initramfs Issue BusyBox 
{% endhint %}

![](../.gitbook/assets/image.jpg)

> solution

```text
fsck /dev/sda1
```

 `/dev/sda1` is the first partition of first drive. **sda**  may change

```text
reboot
```

{% hint style="danger" %}
Date and Time setting
{% endhint %}

> Solution

![](../.gitbook/assets/image2.jpg)

```text
sudo date 010224311971.59
```

> OR

```text
sudo date --set="2020-01-02 23:31:5
```

{% hint style="danger" %}
Minimal bash like Line editing is supported/GRUB Issue
{% endhint %}

![](../.gitbook/assets/pic.jpg)

> solution:

