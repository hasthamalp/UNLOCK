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

 **Remove Token Drivers**

{% tabs %}
{% tab title="PROXKey" %}
```text
sudo apt-get purge wdtokentool-proxkey
```
{% endtab %}

{% tab title="ePass" %}

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

