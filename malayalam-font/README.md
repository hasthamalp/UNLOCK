---
icon: keyboard
---

# 6. Malayalam Typing

Swathanthra Malayalam Computing (SMC) is a free software collective engaged in development, localization, standardization and popularization of various **Free and Open Source** Softwares in Malayalam language.

{% embed url="https://smc.org.in/fonts/" %}



![](../.gitbook/assets/Inscript.jpg)

**Malayalam Inscript Typing**:writing\_hand: [malayalm-typing.pdf](https://icfoss.in/doc/malayalam-typing.pdf)

<div align="left"><img src="https://img.shields.io/badge/courtesy-ICFOSS-34626c" alt=""></div>

#### 2022-ലെ ലിപിപരിഷ്കരണ നിർദേശപ്രകാരമുള്ള മലയാളംഫോണ്ടുകൾ

{% embed url="https://kerala.gov.in/malayalamfont" %}

ലിപി പരിഷ്കരിച്ചുകൊണ്ടുള്ള 2022 മെയ് 9 ലെ സർക്കാർ [ഉത്തരവ്](https://ia802502.us.archive.org/3/items/malayalam-script-reformation-2022/Malayalam%20Script%20Reformation%202022.pdf)

<figure><img src="../.gitbook/assets/imagelipi.png" alt=""><figcaption></figcaption></figure>

## Government And Unicode

എല്ലാ സർക്കാർ ഓഫീസുകളും യുണീക്കോഡധിഷ്ഠിത മലയാളം ഉപയോഗിക്കണമെന്ന 2008 ലെ സർക്കാർ ഉത്തരവ് [ go.pdf](https://go.lsgkerala.gov.in/files/go20081110_6255.pdf)

#### യൂണികോഡിനെ കുറിച്ച് കൂടുതൽ അറിയാൻ&#x20;

{% embed url="https://home.unicode.org" %}

## ചില്ലക്ഷരങ്ങൾ

| <mark style="color:blue;">**ചില്ലക്ഷരങ്ങൾ**</mark> | <mark style="color:blue;">**Inscript key**</mark> |
| -------------------------------------------------- | ------------------------------------------------- |
| **ൾ**                                              | **N+d+]**                                         |
| **ർ**                                              | **j+d+]**                                         |
| **ൻ**                                              | **v+d+]**                                         |
| **ൺ**                                              | **C+d+]**                                         |
| **ൽ**                                              | **n+d+]**                                         |

![](../.gitbook/assets/windows.png)

## **വിൻഡോസിൽ ചില്ലക്ഷരം ഉപയോഗിക്കേണ്ട വിധം**

| <mark style="color:blue;">**ചില്ലക്ഷരം**</mark> | <mark style="color:blue;">**Short Key**</mark> | <mark style="color:blue;">**Inscript**</mark> <mark style="color:blue;">**Key**</mark> |
| ----------------------------------------------- | ---------------------------------------------- | -------------------------------------------------------------------------------------- |
| **ൾ**                                           | **SHIFT+8**                                    | **N+d+Ctrl+Shift+1**                                                                   |
| **ർ**                                           | **]**                                          | **j+d+Ctrl+Shift+1**                                                                   |
| **ൻ**                                           | **SHIFT+v**                                    | **v+d+Ctrl+Shif**&#x74;**+1**                                                          |
| **ൺ**                                           | **SHIFT+x**                                    | **C+d+Ctrl+Shift+1**                                                                   |
| **ൽ**                                           | **SHIFT+ .(dot)**                              | **n+d+Ctrl+Shift+1**                                                                   |

## ചില്ലക്ഷരം ലഭിക്കാന്‍ എന്ത് ചെയ്യണം?

{% hint style="info" %}
**ഗ്നു/ലിനക്സ്** ആണ് ഉപയോഗിക്കുന്നതെങ്കില്‍ **അടിസ്ഥാന അക്ഷരവും ചന്ദ്രക്കല പിന്നെ ]** ചേര്‍ന്നാല്‍ ചില്ലക്ഷരം കിട്ടും. ഉദാ: ല ് ] = ല്‍; ന ് ] = ന്‍; ര ് ] = ര്‍&#x20;
{% endhint %}

![](../.gitbook/assets/shortkey.JPG)

{% hint style="info" %}
**വിന്‍ഡോസാണെങ്കില്‍ ] നു പകരം Ctrl + shift + 1** ഉപയോഗിക്കാം. ഉദാ: ല ് ctrl + shift + 1 = ല്‍&#x20;
{% endhint %}

#### Zero Width Joiner (ZWJ)

{% hint style="info" %}
**കീബോര്‍ഡിലെ ]** കീയുടെ സ്ഥാനത്താണ് zwj. ചില്ലക്ഷരങ്ങല്‍ക്കു വേണ്ടിയാണ് ഇത് ഉപയോഗിക്കുന്നത്.

ഉദാ: ല ് ] = ല്‍, ര ് ] = ര്‍, ന ് ] = ന്‍ etc.
{% endhint %}

#### Zero Width Space (ZWS)

{% hint style="info" %}
**X കീയുടെ സ്ഥാനത്താണ് zws.** രണ്ട് അക്ഷരങ്ങള്‍ക്കിടയില്‍ അദൃശ്യമായ space വേണമെങ്കില്‍ ഇതുപയോഗിക്കാം.

ഉദാ: ക്ക എന്നത് ക​് ക എന്നെഴുതാന്‍
{% endhint %}

#### Zero Width Non Joiner (ZWNJ)

{% hint style="info" %}
&#x20;**\ കീയുടെ സ്ഥാനത്താണ് zwnj.** അടുത്തുവരുന്ന രണ്ട് അക്ഷരങ്ങള്‍ യോജിപ്പിക്കെണ്ടെന്നുണ്ടെങ്കില്‍ ഇതുപയോഗിക്കാം.

ഉദാ: സോഫ്റ്റ്​​വെയര്‍ എന്നെഴുതാന്‍ സോഫ്റ്റ് ന് ശേഷം zwnj ഇല്ലെങ്കില്‍ സോഫ്റ്റ്വെയര്‍ എന്നാകും വരുക.
{% endhint %}

<div align="left"><img src="https://img.shields.io/badge/courtesy-http%3A%2F%2Fmalayalam.kerala.gov.in%2F-34626c" alt=""></div>

## MS Word ൽ അക്ഷരങ്ങൾ തമ്മിൽ അകലം

{% hint style="info" %}
:police\_officer: മലയാളം ഫോണ്ടുകൾ ഉപയോഗിക്കുമ്പോൾ ഇംഗ്ലീഷ് ഉള്ളടക്കം വരുന്നിടത്ത് അക്ഷരങ്ങൾ തമ്മിൽ അനാവശ്യ അകലം വന്നേക്കാം. ഉദാഹരണത്തിന് j എന്ന അക്ഷരത്തിന് മുമ്പ് സ്പേസ് ഇട്ടപോലെ അകലം കാണാം. ഈ പ്രശ്നം വേഡ് 2013 ൽ സാധാരണമാണ്. ഇത് പരിഹരിക്കാൻ വേഡിലെ Kerning എന്ന ഫീച്ചർ ഇനേബിൾ ചെയ്യണം.

&#x20;അതിനായി ഈ [<mark style="color:green;">ലേഖനം</mark>](https://www.dummies.com/software/microsoft-office/word/how-to-enable-kerning-in-word-2013-documents/) ഉപകരിക്കും.
{% endhint %}

## ചില്ലുകൾക്ക് പകരം രെജിസ്റ്റേഡ് ചിഹ്ന&#xD02;**®**

{% hint style="info" %}
:woman\_guard:  2010 ന് മുമ്പ് പുറത്തിറങ്ങിയ രചന, മീര തുടങ്ങിയ ഫോണ്ടുകളിൽ അറ്റോമിക് ചില്ലുകൾക്ക് പകരം വട്ടത്തിനകത്തെ &#x52;**(®)** എന്ന രൂപമാണ് കാണുക. അറ്റോമിക് ചില്ലുകൾ വരുന്നതിനു മുമ്പ് പുറത്തിറങ്ങിയ പതിപ്പായതാണ് ഇതിനു കാരണം. ആ ഫോണ്ടുകളുടെ [<mark style="color:green;">പുതിയ പതിപ്പുകൾ ഇൻസ്റ്റാൾ ചെയ്താൽ ഈ പ്രശ്നം പരിഹരിക്കാം.</mark>](https://smc.org.in/fonts/)
{% endhint %}

## [**POORNA Keyboard**](https://poorna.smc.org.in)

{% hint style="info" %}
Poorna is a keyboard layout which includes all the Malayalam Unicode characters.These are available in two variants:Inscript and Remington
{% endhint %}

## **Enabling Malayalam language UI in Ubuntu**

Click `Setting` > `Region and Language` > `Manage installed languages` .

![](../.gitbook/assets/img11.JPG)

You can click `Remind me later` Otherwise you can install the additional recommendations and return to this screen.

![](https://smc.org.in/articles/images/ubuntu.20.04/language_support_2.png)

Now click on `Install/Remove languages` and scroll till you find Malayalam.

![](https://smc.org.in/articles/images/ubuntu.20.04/language_support_3.png)

Make sure the `Malayalam` is selected. Now click `Apply`. It will ask your password for permission to install language support.

Once it finishes, make sure **`മലയാളം`** is visible in the list as per below.

![](https://smc.org.in/articles/images/ubuntu.20.04/language_support_4.png)

Now click close, and you should be back at Region and Language screen. Close this screen, and launch `Settings` again, and click on `Region and Languages` > `Languages`.

![](https://smc.org.in/articles/images/ubuntu.20.04/language_support_5.png)

Select `മലയാളം` in the screen and click on the `Select` button.

This will enable the Malayalam UI. You'd need to restart your session (not the computer itself). Clicking on the restart button will log you out.

![](https://smc.org.in/articles/images/ubuntu.20.04/language_support_6.png)

:white\_check\_mark: When you log back in, you should see Malayalam user interface.



> [![SMC](https://img.shields.io/badge/Courtesy-Swathanthra%20Malayalam%20Computing-1B98F5)](https://smc.org.in/)





