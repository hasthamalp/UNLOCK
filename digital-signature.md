---
icon: usb-drive
---

# 3. 🔐 Digital signature

## Digital Signature Driver Software

{% hint style="info" %}
* PROXKey
* ePass
{% endhint %}

## TRACK DSC STATUS

{% embed url="https://ra.care4sign.com/Care4Sign_V1/CommonSearchUploadRecord.jsp" %}

## Care4Sign Software

{% embed url="https://ra.care4sign.com/Care4Sign_V1/dowonloadUtility" %}

## &#x20;**Remove Token Drivers**

{% tabs %}
{% tab title="PROXKey" %}
```
sudo apt-get purge wdtokentool-proxkey
```

```
 cd /usr/lib/WatchData/ProxKey
```

```
sudo ./uninstall 
```
{% endtab %}
{% endtabs %}

## Install Proxkey Token Tool on Ubuntu 24.04

{% hint style="info" %}
Download latest Token driver compactable with Ubuntu 24.04. Then&#x20;

`sudo apt install bzip2`

Install Token Driver
{% endhint %}

## DSC View Certificate

{% tabs %}
{% tab title="epass2003" %}
```
sudo pkimanager_admin
```
{% endtab %}
{% endtabs %}

## Reset ProxKey USER PIN -Proxkey

[Token Unlock](https://manage.cryptoplanet.in/en/):person\_raising\_hand:

Pre Prerequisites for Reset USER PIN

Token must be registered either by following methods

1. **PIN Mode Registration** – Validate Token User PIN (Register token at the time of purchase)
2. **KYC Mode Registration** – Validate Certificate KYC (Use this when token USER PIN is not know)
3. **Manual Mode Registration** – Validate ID Proof & submit application form

## Steps to Reset Token USER PIN

1. Install the token middle ware / driver([visit here](http://www.e-mudhra.com/Repository/index.html))
2. Locate “WD ProxKey” Icon on the desktop and double click on it to open the Token Management Utility
3. Token middle ware interface will open

![](.gitbook/assets/pk1.JPG)

4.Press `Ctrl + Alt + W` to see the Admin menu & click on ‘Unlock User PIN’. You will require to generate an ‘AUTHENTICATION KEY’ . Click on ‘GENERATE

![](.gitbook/assets/pk3.JPG)

You will get a prompt. DO NOT DISCONNECT TOKEN till authentication key is generated. Click on OK

![](.gitbook/assets/pk4.JPG)

You will be redirected to website to Authenticate using OTP on mobile number used while Token Registration. Enter the OTP received on mobile and click on ‘VERIFY OTP

![](.gitbook/assets/pk5.JPG)

You will be displayed your SERIAL NUMBER, AUTHENTICATION KEY & DEFAULT ADMIN PIN. Copy the AUTHENTICATION KEY

![](.gitbook/assets/pk6.JPG)

Paste the key in the token middleware and click on Unlock

![](.gitbook/assets/pk7.JPG)

Enter the default admin pin of the token or use your changed admin pin (In case you have changed your admin pin)

![](.gitbook/assets/pk8.JPG)

RESET OF USER PIN is successful

![](.gitbook/assets/pk9.JPG)

Enter your new USER PIN and click OK

![](.gitbook/assets/pk10.JPG)

![](.gitbook/assets/pk11.JPG)

