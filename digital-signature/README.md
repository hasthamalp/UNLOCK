# 🔐 Digital signature

## Digital Signature Driver Software

{% hint style="info" %}
* DSC Token Driver\(NICDSign\)
* TRUSTKEY
* PROXKey
* ePass
{% endhint %}

#### TRACK DSC STATUS

{% embed url="https://www.certificate.digital/track-dsc-status/" %}

{% embed url="http://dscsupport.reyleon.com/certificate-status-update.php" %}



 **Remove Token Drivers**

{% tabs %}
{% tab title="PROXKey" %}
```text
sudo apt-get purge wdtokentool-proxkey
```

```text
 cd /usr/lib/WatchData/ProxKey
```

```text
sudo ./uninstall 
```
{% endtab %}

{% tab title="TRUSTKEY" %}
```text
cd /usr/lib/WatchData/TRUSTKEY
```

```text
sudo ./uninstall 
```
{% endtab %}

{% tab title="eMudhra Watchdata" %}
```text
cd /usr/lib/WatchData/eMudhra_3.4.3
```

```text
sudo ./uninstall
```
{% endtab %}
{% endtabs %}

## DSC View Certificate

{% tabs %}
{% tab title="Trust key" %}
```text
sudo watchsafe_TRUSTKEY
```
{% endtab %}

{% tab title="emudra" %}
```text
sudo watchsafe_emudhra_3.4.3
```
{% endtab %}

{% tab title="epass2003" %}
```text
sudo pkimanager_admin
```
{% endtab %}
{% endtabs %}

