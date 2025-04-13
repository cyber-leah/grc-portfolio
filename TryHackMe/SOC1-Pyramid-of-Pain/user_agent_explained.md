# 🧠 Understanding User-Agent Strings

A **User-Agent** is a string of text sent by a browser or software to a web server that identifies the application, operating system, and other system details. It helps websites deliver content tailored to the device or software making the request.

---

## 💡 Why User-Agent Strings Matter in Cybersecurity

- Attackers may **spoof** them to evade detection.
- Malware (like Emotet) often uses **custom or suspicious strings**.
- Analysts and SOC teams use them to **detect anomalies** and **investigate intrusions**.

---

## 🔍 User-Agent String Anatomy

| Part | Example | Meaning |
|------|---------|---------|
| `Mozilla/5.0` | `Mozilla/5.0` | Legacy compatibility marker used by most browsers |
| OS Info | `Windows NT 10.0` | Operating system (Windows 10) |
| Platform | `WOW64`, `x64` | System architecture (32-bit/64-bit) |
| Browser Engine | `AppleWebKit/537.36` | Rendering engine (used by Chrome, Safari) |
| Browser Info | `Chrome/113.0.0.0` | Browser and version |
| IE Engine | `Trident/7.0` | Internet Explorer rendering engine (Trident 7 = IE 11) |
| Compatibility | `MSIE 7.0` | Internet Explorer in compatibility mode |
| Extras | `.NET CLR`, `Media Center` | Additional features or installed components |

---

## 🧪 Example Breakdown

### User-Agent:
```
Mozilla/4.0 (compatible; MSIE 7.0; Windows NT 6.1; Trident/7.0; .NET CLR 3.5.30729)
```

| Component | Explanation |
|----------|-------------|
| Mozilla/4.0 | Legacy placeholder |
| MSIE 7.0 | Pretending to be IE 7 |
| Windows NT 6.1 | Running Windows 7 |
| Trident/7.0 | Really Internet Explorer 11 |
| .NET CLR 3.5.30729 | Installed .NET Framework version |

---

## 📚 Related Tools & Links

- [WhatIsMyBrowser.com](https://www.whatismybrowser.com/)
- [MDN Web Docs - User-Agent](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/User-Agent)

---

*Tip: In threat detection, look for unusual or outdated combinations of engines and OSes that don't match normal user behavior.*
