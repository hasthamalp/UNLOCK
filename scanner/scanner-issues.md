# Scanner Issues

Try below method for <mark style="background-color:green;">HP  plugin issues</mark>. first _install HPLIP latest version_ on system and try following steps.

Download Latest [Plugins](https://developers.hp.com/hp-linux-imaging-and-printing/plugins) from HP website: version may vary

Run this command to Install Plugin:

```shell
sh hplip-3.24.4-plugin.run
```

{% hint style="success" %}
That fixed the Scanner issue.Now you able to scan without any issues.:smile:
{% endhint %}

### Epson WorkForce DS-530II Scanner Package Missing Issue

```
sudo apt-get install libqt5gui5
```

Restart your system and try again, scan  working fine. :smile:
