# 6. Printer

![](../.gitbook/assets/35069-printererror.gif)

## Identify installed printers in  system

```text
lpstat -a
```

**How do I remove hundreds of automatically added network printers**

```text
sudo nautilus
```

> Go to `etc`--&gt;`cups-->cups-browsed.conf`



> stop cups and then remove the printers from the file

```text
sudo service cups-browsed stop
```

## ADDING A NETWORK PRINTER \(UBUNTU\)

> 1. `System Settings --> Printers`
>
> 2.     Click `Add` and select `Find Network Printer`
>
> 3.     Enter the `IP address` in the `Host` field, and click `Find.`
>
> 4.       Click `Forward` and wait while the system searches for drivers
>
> 5.        Click `Apply` to finish

## 

