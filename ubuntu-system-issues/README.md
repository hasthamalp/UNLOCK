# 4. Issues and Solutions

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

{% hint style="danger" %}
**Did not find a connection with UUID '\(null\)'**
{% endhint %}

soln:

```text
sudo systemctl stop NetworkManager.service
```

```text
sudo systemctl start NetworkManager.service
```

{% hint style="success" %}
problem solved
{% endhint %}

{% hint style="danger" %}
Your Connection is not secure 
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
Error editing connection:Did not find a connection with UUID '\(null\)'
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

