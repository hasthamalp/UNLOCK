# Network Debugging Techniques

{% hint style="danger" %}
**Error editing connection:Did not find a connection with UUID '\(null\)'**
{% endhint %}

**solution**:

```text
sudo systemctl stop NetworkManager.service
```

```text
sudo systemctl start NetworkManager.service
```

