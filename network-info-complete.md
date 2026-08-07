# Network Information

| Field         | Value              |
|---------------|--------------------|
| **MAC Address** | `XX:XX:XX:XX:XX:XX` |
| **IP Address**  | `192.168.X.X`      |
| **Device Name**  | `your-device-name` |
| **Date**         | `2026-08-07`       |

---

## Apna MAC / IP Address Kaise Nikalein

### Windows
```
ipconfig /all
```
- **IPv4 Address** wahan aapka IP hai
- **Physical Address** wahan aapka MAC hai

### Mac / Linux
```
ifconfig
```
ya
```
ip addr show
```

*Upar table mein `XX:XX:XX:XX:XX:XX` aur `192.168.X.X` ki jagah apna asal MAC/IP daal dein.*

---

## Zip / Tar File Banane Ke Commands

### Zip banane ke liye
```bash
zip -r network-info.zip network-info.md
```

### Tar.gz banane ke liye
```bash
tar -czvf network-info.tar.gz network-info.md
```

### Zip extract karne ke liye
```bash
unzip network-info.zip
```

### Tar.gz extract karne ke liye
```bash
tar -xzvf network-info.tar.gz
```

---

## GitHub Par Push Karne Ke Commands

```bash
git add network-info.md
git commit -m "Add network info file"
git push origin main
```
