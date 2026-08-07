# Linux Basic Commands

## Introduction

Linux provides many useful commands to check system information, disk space, hardware, and system logs. These commands are commonly used by Linux users and system administrators.

---

# 1. Check Disk Space

## df -h

Displays disk space usage in a human-readable format.

```bash
df -h
```

Example Output:

```text
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        50G   18G   30G   38% /
```

---

# 2. Check Directory Size

## du -sh

Shows the total size of a directory.

```bash
du -sh /home
```

Example Output:

```text
2.5G    /home
```

---

# 3. Check Memory Usage

## free -h

Displays RAM and swap memory usage.

```bash
free -h
```

Example Output:

```text
              total   used   free
Mem:           8Gi    3Gi    5Gi
Swap:          2Gi    0Gi    2Gi
```

---

# 4. Check System Uptime

## uptime

Shows how long the system has been running.

```bash
uptime
```

Example Output:

```text
15:30:20 up 3 days, 4:15, 2 users, load average: 0.10, 0.15, 0.12
```

---

# 5. Kernel & System Information

## uname -a

Displays kernel version and system architecture.

```bash
uname -a
```

---

# 6. CPU Information

## lscpu

Displays processor information.

```bash
lscpu
```

---

# 7. Block Devices

## lsblk

Lists all disks and partitions.

```bash
lsblk
```

Example Output:

```text
NAME   SIZE TYPE MOUNTPOINT
sda     50G disk
├─sda1  50G part /
```

---

# 8. System Log Directory

Linux log files are stored in:

```bash
/var/log
```

List log files:

```bash
ls /var/log
```

Common log files:

- syslog
- auth.log
- kern.log
- boot.log
- dmesg

---

# 9. View System Logs

## journalctl

Displays all system logs.

```bash
journalctl
```

View the latest logs:

```bash
journalctl -n 20
```

Follow logs in real time:

```bash
journalctl -f
```

Press **Ctrl + C** to stop monitoring.

---

# Summary

| Command | Description |
|---------|-------------|
| `df -h` | Display disk space usage |
| `du -sh` | Display directory size |
| `free -h` | Show memory usage |
| `uptime` | Show system uptime |
| `uname -a` | Show kernel and system information |
| `lscpu` | Display CPU details |
| `lsblk` | List disks and partitions |
| `ls /var/log` | List log files |
| `journalctl` | View system logs |
| `journalctl -f` | Monitor logs in real time |

---

# Conclusion
174
175
176
177
178
179
180
181
182
183
184
185
186
187
188
189
190
191
192
193
194
195
196
197
These Linux commands are essential for checking disk space, memory usage, CPU information, storage devices, and system logs. They are widely used in Linux administration, troubleshooting, and server management.
