# Adobe Reader

![](../.gitbook/assets/adobe_reader_vertical.png)

## **How to Set Adobe Reader as default PDF reader**

> Run command below in terminal to edit the`config` file:

```text
sudo gedit /etc/gnome/defaults.list
```

> When the file opens, do: Find out and change the line

`application/pdf=evince.desktop`

> into:

```text
application/pdf=acroread.desktop
```

> Add below line into the end:

```text
application/fdf=acroread.desktop
application/xdp=acroread.desktop
application/xfdf=acroread.desktop
application/pdx=acroread.desktop
```

> ✅ Finally save the file and restart nautilus \(run command nautilus -q in terminal\) to apply changes.

