# Phishing URL Detector 🔐

A beginner-friendly cybersecurity project built with Python that analyzes URLs for suspicious patterns commonly associated with phishing attacks.

## 📌 About the Project

Phishing is a cyberattack in which attackers use deceptive links to trick people into revealing sensitive information. This project checks URLs for potential warning signs and generates a simple risk indicator.

This tool is designed for educational purposes and helps beginners understand basic phishing detection techniques.

## ✨ Features

- Detects URLs that use IP addresses instead of domain names.
- Checks whether a URL uses HTTPS.
- Identifies unusually long URLs.
- Flags potentially misleading URLs containing the `@` symbol.
- Detects hostnames with many domain labels.
- Checks for suspicious login-related keywords.
- Identifies URLs from a small list of URL-shortening services.
- Calculates a simple risk score.
- Displays warnings and findings in the terminal.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:** `urllib.parse`, `ipaddress`, `re`
- **Additional Installation:** None required

## 📋 Requirements

- Python 3.10 or newer recommended
- Windows, Linux, or macOS
- A terminal or command prompt

## 🚀 Installation and Usage

### 1. Clone the Repository

Replace `YOUR-USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR-USERNAME/phishing-url-detector.git
```

### 2. Open the Project Folder

```bash
cd phishing-url-detector
```

### 3. Run the Program

```bash
python phishing_detector.py
```

### 4. Enter a Test URL

Enter a URL when the program prompts you. The application displays a risk indicator and any warnings detected by its rules.

## 🧪 Example Test Cases

| Test URL | Purpose |
|---|---|
| `https://example.com` | Test a standard HTTPS URL |
| `http://192.0.2.1/login` | Test an IP-based hostname |
| `http://example.com@192.0.2.1` | Test a potentially misleading URL |
| `https://bit.ly/example` | Test a URL-shortening service |

These examples are for testing only. The IP address `192.0.2.1` is reserved for documentation.

## 📊 Risk Score

The program produces a score from 0 to 10.

- **0–2:** Few configured warning indicators
- **3–5:** Caution
- **6–10:** High risk indicators

The score is based on simple rules and is not a scientifically validated probability of phishing.

## ⚠️ Limitations

- A legitimate website may trigger warnings.
- A phishing website may not trigger any warnings.
- HTTPS does not guarantee that a website is trustworthy.
- The program does not verify website reputation or check live threat-intelligence databases.
- URL shortening alone does not mean a link is malicious.

## 🔒 Security Disclaimer

This project is intended for cybersecurity education and defensive analysis.

Do not open suspicious links to test them. Use fictional URLs or trusted test data. Do not enter passwords or other sensitive information into untrusted websites.

## 🎯 Future Improvements

- Add a graphical user interface.
- Improve domain and hostname analysis.
- Add unit tests.
- Integrate reputable threat-intelligence services.
- Generate downloadable analysis reports.
- Improve risk scoring using a validated detection model.

## 👨‍💻 Author

Created as a student cybersecurity learning project.

## 📄 License

This project is available under the MIT License. If you choose this license, add a `LICENSE` file containing the standard MIT License text and your chosen copyright notice.
