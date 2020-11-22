# Share

#### ഉബുണ്ടു സിസ്റ്റത്തിൽ Share ഇൻസ്റ്റാൾ ചെയ്യാം

![](../.gitbook/assets/folder2_39672.png)

```text
sudo apt-get install nfs-common
```

```text
sudo apt-get -f install   
```

## create a directory called _share_

```text
mkdir share
```

```text
sudo nautilus  
```

{% hint style="info" %}
`computer`-&gt;`etc`-&gt;`fstab`-&gt;`10.69.51.20:`//share \(tab\)/`home`/`(computername)`/`share` \(tab\) `nfs` \(tab\) `auto` \(tab\) `0` \(tab\) `0`-&gt;`save`.
{% endhint %}

```text
sudo mount -a   
```

{% hint style="success" %}
SHARE  is now done successfully on your system
{% endhint %}

