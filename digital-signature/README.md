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

![](../.gitbook/assets/pk3.jpg)

You will get a prompt. DO NOT DISCONNECT TOKEN till authentication key is generated. Click on OK

![](../.gitbook/assets/pk4.jpg)

You will be redirected to website to Authenticate using OTP on mobile number used while Token Registration. Enter the OTP received on mobile and click on ‘VERIFY OTP

![](../.gitbook/assets/pk5.jpg)

You will be displayed your SERIAL NUMBER, AUTHENTICATION KEY & DEFAULT ADMIN PIN. Copy the AUTHENTICATION KEY

![](../.gitbook/assets/pk6.jpg)

Paste the key in the token middleware and click on Unlock

![](../.gitbook/assets/pk7.jpg)

Enter the default admin pin of the token or use your changed admin pin \(In case you have changed your admin pin\)

![](../.gitbook/assets/pk8.jpg)

RESET OF USER PIN is successful

![](../.gitbook/assets/pk9.jpg)

Enter your new USER PIN and click OK

![](../.gitbook/assets/pk10.jpg)

