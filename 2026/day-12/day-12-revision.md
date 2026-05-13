# Day 12 – Revision & Breather

## Revision Summary

Today I revised the core Linux and DevOps fundamentals learned from Days 01–11.

---

# Mindset & Learning Plan Review

- My long-term goal is still to become a strong DevOps Engineer.
- I want to improve Linux speed, command confidence, and troubleshooting.
- Need more practice with permissions and process monitoring.
- Feeling much more comfortable with terminal usage compared to Day 01.

---

# Processes & Services Revision

## Commands Practiced

### Process Monitoring

```bash
ps aux
```

Observation:
- Displays all running processes with CPU and memory usage.

### Service Status

```bash
systemctl status docker
```

Observation:
- Shows whether Docker service is active or failed.

### Logs Checking

```bash
journalctl -u docker -n 20
```

Observation:
- Helps identify service-related logs and troubleshooting information.

---

# File Skills Revision

## Commands Practiced

### Append Text

```bash
echo "DevOps Practice" >> notes.txt
```

### Change Permissions

```bash
chmod 755 script.sh
```

### Change Ownership

```bash
sudo chown tokyo:vault-team access-codes.txt
```

### Create Directory

```bash
mkdir project-files
```

### Copy Files

```bash
cp notes.txt backup-notes.txt
```

---

# Top 5 Most Useful Commands

| Command | Why Useful |
|---|---|
| `ls -l` | View permissions and ownership quickly |
| `ps aux` | Check running processes |
| `journalctl` | Troubleshoot services using logs |
| `chmod` | Control file permissions |
| `chown` | Manage ownership in multi-user systems |

---

# User & Group Practice

## Scenario Recreated

Created a test user and changed ownership of a file.

Commands used:

```bash
sudo useradd testuser
touch practice.txt
sudo chown testuser practice.txt
ls -l practice.txt
id testuser
```

Observation:
- Ownership successfully changed to `testuser`.

---

# Mini Self-Check

## 1. Which 3 commands save you the most time right now, and why?

- `ls -l` → instantly shows permissions and ownership
- `ps aux` → helps monitor running processes
- `journalctl` → useful for troubleshooting service issues

---

## 2. How do you check if a service is healthy?

Commands:

```bash
systemctl status docker
ps aux | grep docker
journalctl -u docker -n 20
```

---

## 3. How do you safely change ownership and permissions?

Example:

```bash
sudo chown ubuntu:ubuntu app.log
chmod 644 app.log
```

This safely changes:
- owner/group
- readable permissions without making file executable unnecessarily

---

## 4. What will you focus on improving in the next 3 days?

- Faster Linux command usage
- Better troubleshooting skills
- More confidence with permissions and services
- Shell scripting basics

---

# Key Takeaways

- Linux permissions are extremely important in DevOps.
- Logs are critical for troubleshooting.
- Ownership and groups control secure collaboration.
- Practicing commands repeatedly improves confidence.
- Understanding services/processes is foundational for servers.

---

# Overall Progress

Completed revision of Days 01–11 successfully.
Feeling more comfortable using Linux daily.