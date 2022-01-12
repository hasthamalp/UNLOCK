# DSC Issues

### Add DSC token driver(ePass) in NICDSign(for BIMS/SPARK)

Right-click on the Rubix cube and select Settings and select the correct dsc token `(proxkey / epass )`

{% hint style="info" %}
For **epass,** select `custom`---> Then click on the `browse file` below. ** `C: \ Windows \ System32 \eps2003csp11.dll`** and **save**
{% endhint %}

&#x20; **Just save to Proxkey.**

![](../.gitbook/assets/IMG\_20220112\_142202\_mfnr.jpg)

{% hint style="success" %}
When you save it you will be asked to re-insert the token. When done, the dsc token and signer are ready.
{% endhint %}

## Proxkey Library Implementation Process

#### select your PKCS#11 Implementation library in <mark style="background-color:orange;"></mark> <mark style="background-color:orange;"></mark><mark style="background-color:orange;">**Linux**</mark>

{% hint style="info" %}
`usr--->lib--->watchData--->Proxkey--->lib-->libwdpkcs_SignatureP11.so`
{% endhint %}

#### select your PKCS#11 Implementation library in <mark style="background-color:blue;">Windows</mark>

{% hint style="info" %}
for windows the file will be in  **C:\windows\system32**

**------>SignatureP11.dll**
{% endhint %}

![](../.gitbook/assets/IMG\_20220112\_142152\_mfnr.jpg)
