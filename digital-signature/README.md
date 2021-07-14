# 2. 🔐 Digital signature

## Digital Signature Driver Software

{% hint style="info" %}
* DSC Token Driver\(NICDSign\)
* TRUSTKEY
* PROXKey
* ePass
{% endhint %}

## TRACK DSC STATUS

{% embed url="https://www.certificate.digital/track-dsc-status/" %}

{% embed url="http://dscsupport.reyleon.com/certificate-status-update.php" %}

## Download Token Driver

{% embed url="http://www.e-mudhra.com/Repository/index.html" %}



##  **Remove Token Drivers**

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

## Reset ProxKey USER PIN

Pre Prerequisites for Reset USER PIN

Token must be registered either by following methods

1. **PIN Mode Registration** – Validate Token User PIN \(Register token at the time of purchase\)
2. **KYC Mode Registration** – Validate Certificate KYC \(Use this when token USER PIN is not know\)
3. **Manual Mode Registration** – Validate ID Proof & submit application form

## Steps to Reset Token USER PIN

1. Install the token middle ware / driver\([visit here](http://www.e-mudhra.com/Repository/index.html)\)
2. Locate “WD ProxKey” Icon on the desktop and double click on it to open the Token Management Utility
3. Token middle ware interface will open

![](../.gitbook/assets/pk1.jpg)

4.Press `Ctrl + Alt + W` to see the Admin menu & click on ‘Unlock User PIN’. You will require to generate an ‘AUTHENTICATION KEY’ . Click on ‘GENERATE

