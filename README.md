# ~/yash_vinchhi/portfolio

> Software Developer & Designer

Building aesthetic, robust applications and seamless user experiences. Bridging the gap between engineering and design.

---

## 🚀 Selected Work

### [AttendX](https://attendx.ripaldesign.studio/)
Attendance tracking platform built for modern organizations.
- **Type:** WebApp

### [Ripal Design Studio](https://ripaldesign.studio/)
Creative portfolio and studio website showcasing design excellence.
- **Type:** Portfolio

### Mobile App
Download my latest mobile application build.
- **Type:** Android / Download
- *(Link pending)*

---

## 📬 Contact & Connect

- **WhatsApp:** [+91 79844 17971](https://wa.me/917984417971)
- **Primary Phone:** [+91 79844 17971](tel:+917984417971)
- **Secondary Phone:** [+91 94288 65525](tel:+919428865525)
- **Email:** [yashhvinchhi@gmail.com](mailto:yashhvinchhi@gmail.com)

---

## 🔗 Socials

- [GitHub (Main)](https://github.com/YashVinchhi)
- [GitHub (Alt)](https://github.com/yvinchhi)
- [LinkedIn](https://www.linkedin.com/in/yash-h-vinchhi/)
- [X (Twitter)](https://x.com/yashhvinchhi)
- [Instagram](https://www.instagram.com/yeaas_vinchhi/)

---

## 📡 NFC Tracking Setup (Server-Side)

This landing page is designed to be written to an NFC card and hosted on an Ubuntu server (`Yash.ripaldesign.studio`). It tracks card usage with zero front-end overhead.

### How it Works:
1. Program your NFC cards to point to your URL with a unique query parameter.
   - Example Card 1: `https://Yash.ripaldesign.studio/?nfc=card_01`
   - Example Card 2: `https://Yash.ripaldesign.studio/?nfc=card_02`
2. When a user taps the card, the browser requests the URL.
3. The Ubuntu web server (Nginx/Apache) automatically logs this request in its `access.log`.

### Checking Analytics:
To see how many times a specific card was scanned, SSH into your Ubuntu server and run:

**For Nginx:**
```bash
grep "nfc=card_01" /var/log/nginx/access.log | wc -l
```

**For Apache:**
```bash
grep "nfc=card_01" /var/log/apache2/access.log | wc -l
```