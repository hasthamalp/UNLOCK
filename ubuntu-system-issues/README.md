# 5. Issues and Solutions

![](../.gitbook/assets/27659-bug-guy-1-.gif)

{% hint style="danger" %}
**1**.Initramfs Issue BusyBox 
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
**2**.failed to start nvidia persistence daemon
{% endhint %}

![](../.gitbook/assets/500089300355_338398.jpg)

solution: first restart your system. then select `ubuntu` from GRUB menu. then press the `E` key. Add `nouveau.modeset=0` to the end of the `linux` line - press `F10` to boot.

{% hint style="info" %}
 `nomodeset` is a temporary solution in case a system does not boot without a proprietary driver. This is not to be used permanently.
{% endhint %}

{% hint style="danger" %}
**3**.Date and Time setting
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
**4.**Minimal bash like Line editing is supported/GRUB Issue
{% endhint %}

![](../.gitbook/assets/pic.jpg)

> solution:

{% hint style="danger" %}
**5.**Your Connection is not secure 
{% endhint %}

> problem

![](../.gitbook/assets/bb87bd14-b11a-4f38-bcc1-d053a9d6609f.jpg)

> solution

click **`Advanced`** option

![](../.gitbook/assets/0dee2d45-d936-417b-abc2-401c842eb369.jpg)

click **`Add Exception`** option

![](../.gitbook/assets/74ee58a8-e872-4a6f-92f6-de7993c444f7.jpg)

![](../.gitbook/assets/exception.jpg)

✅ success

{% hint style="danger" %}
**6.**Error editing connection:Did not find a connection with UUID '\(null\)'
{% endhint %}

solution:

```text
sudo systemctl stop NetworkManager.service
```

```text
sudo systemctl start NetworkManager.service
```

How do I change the user account password?

```text
passwd
```

To change other users password:

```text
sudo passwd USERNAME
```

