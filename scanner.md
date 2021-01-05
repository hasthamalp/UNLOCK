# Scanner

![](.gitbook/assets/8898-document-scanner.gif)

## How to install XSANE in Ubuntu

```text
sudo apt install xsane
```

**You must install the mono package to complete the scanner installation**

{% tabs %}
{% tab title="Ubuntu 20.04" %}
```text
sudo apt install gnupg ca-certificates
```

```text
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
```

```text
echo "deb https://download.mono-project.com/repo/ubuntu stable-focal main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list
```

```text
sudo apt update
```
{% endtab %}

{% tab title="Ubuntu 18.04" %}
```text
sudo apt install gnupg ca-certificates
```

```text
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
```

```text
echo "deb https://download.mono-project.com/repo/ubuntu stable-bionic main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list
```

```text
sudo apt update
```
{% endtab %}
{% endtabs %}

> Identify which scanner is used

```text
scanimage -L
```



