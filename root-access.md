# 🔐 How to Become Root in Linux

In Linux, **root** is the superuser account with full administrative access. Here's how to gain root privileges safely.

---

## ✅ 1. Using `sudo` (Temporary Root Privileges)

Most modern distributions (like Ubuntu, Kali) use `sudo`:

```bash
sudo command
```

🔹 Example:
```bash
sudo apt update
```

- Prompts for your user password
- Runs **only that command** as root

---

## ✅ 2. Permanent Root Shell (Use with Caution)

You can start a root shell for multiple root-level commands:

```bash
sudo -i
```
or
```bash
sudo su
```

You now have a **persistent root shell**. Be extra careful — every command now has superuser rights.

🔸 To exit root shell:
```bash
exit
```

---

## ✅ 3. Root Login (If Allowed)

If your system allows logging in as root:

```bash
su -
```

You will need the **root password**, which may not be set by default.

---

## ⚠️ Warning

Root access allows you to:
- Delete system files
- Change critical settings
- Install/remove software globally

🛑 Always double-check your commands when running as root.

---

## 📌 Pro Tip

To check if you're root, use:

```bash
whoami
```

If it returns `root`, you are currently in superuser mode.

---

Stay safe and happy hacking! 😄
