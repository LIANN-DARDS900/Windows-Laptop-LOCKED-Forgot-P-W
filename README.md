# 🔐 Windows Password Recovery Guide using Hiren’s BootCD PE

This educational guide provides a step-by-step method to reset or recover a forgotten local Windows administrator password using [Hiren’s BootCD PE](https://www.hirensbootcd.org/). It is intended for IT professionals, technicians, and system administrators who need to regain access to authorized systems.

> ⚠️ **Disclaimer:** This guide is for educational purposes only. Do not use it to access systems you do not own or have explicit permission to maintain. Unauthorized access is illegal and unethical.

---

## 📦 What You'll Need

- A USB flash drive (minimum 4 GB)
- [Hiren’s BootCD PE ISO](https://www.hirensbootcd.org/download/)
- [ISO2USB Tool](https://www.hirensbootcd.org/usb-booting/)

---

## 🛠️ Step-by-Step Instructions

1. **Download the ISO**  
   Get the latest version of Hiren’s BootCD PE from the official website.

2. **Create a Bootable USB**  
   Use the ISO2USB tool to write the ISO to your USB drive.

3. **Boot the Target PC**  
   Insert the USB into the locked computer and boot from it (usually by pressing `F12`, `ESC`, or `DEL` during startup).

4. **Launch NT Password Edit**
   - Navigate to:  
     `Start Menu → Utilities → Security → NT Password Edit`
   - Open the SAM file:  
     `C:\Windows\System32\config\SAM`
   - Select the user account.
   - Click "Change Password" (leave it blank to remove the password).
   - Save changes and close the tool.

5. **Reboot Without USB**  
   The system should now allow login without a password (or with the new one you set).

---

## ❗ Important Notes

- This works only for **local Windows accounts** (not Microsoft online accounts).
- It **does not work** on drives encrypted with BitLocker unless the recovery key is available.
- No data will be deleted during this process.

---

## 📚 License

This guide is released under the [MIT License](./LICENSE). Use it responsibly.

---

## 🙏 Acknowledgements

- [Hiren’s BootCD PE](https://www.hirensbootcd.org/)
- Hiren's team and contributors for creating this powerful recovery environment.
