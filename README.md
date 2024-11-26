<p align="center">
  <img src="https://i.imgur.com/TsYw7b9.png" alt="Google-Hacking-Database" />
</p>

# Google Dorking: A Comprehensive Guide

Welcome! This repository is dedicated to learning everything about **Google Dorking**, a powerful technique for extracting specific information using search engines. This document is designed for educational purposes and cybersecurity awareness.

---

## 📖 What is Google Dorking?

**Google Dorking** (or Google Hacking) is a technique that uses advanced search operators in search engines, like Google, to locate sensitive information that might have been unintentionally exposed online. This includes:

- Confidential files.
- Pages with login credentials.
- Server configurations.
- Exposed network devices.

⚠️ **Note:** Google Dorking must be used ethically and legally. Improper use may lead to severe consequences.

---

## 🛠 Basic Search Operators

| **Operator**    | **Description**                                        | **Example**                          |
|------------------|-------------------------------------------------------|--------------------------------------|
| `site:`         | Limits results to a specific domain.                  | `site:example.com`                  |
| `intitle:`      | Searches for keywords in the page title.              | `intitle:"login"`                   |
| `inurl:`        | Searches for keywords in the URL.                     | `inurl:"admin"`                     |
| `filetype:`     | Searches for specific file types.                     | `filetype:pdf "confidential"`       |
| `ext:`          | Short version of `filetype:`.                         | `ext:docx "password"`               |
| `cache:`        | Displays the cached version of a page.                | `cache:example.com`                 |
| `" "`           | Matches an exact phrase.                              | `"index of /"`                      |

---

## 🔍 Common Google Dorking Examples

- Find exposed configuration files:

```text
  filetype:env "DB_PASSWORD"
```

- List open directories:
    
    ```text
    intitle:"index of" "parent directory"
    ```
    
- Search for accessible IP cameras:
    
    ```text
    inurl:"/view/index.shtml"
    ```
    
- Credentials on GitHub:
    
    ```text
    site:github.com "AWS_SECRET_ACCESS_KEY"
    ```
    

---

## 🛡 Prevention Measures

To protect your assets from Google Dorking:

1. **Configure robots.txt**: Limit search engines' access to sensitive areas of your website.
2. **Avoid posting sensitive data online**: Never publish credentials or configuration files in public repositories.
3. **Use vulnerability scanners**: Regularly audit your assets to identify exposed data.
4. **Set proper permissions**: Protect sensitive directories and files with passwords or restricted access.
5. **Monitor your online presence**: Use tools like Google Alerts to detect exposed data.

---

## 💻 Complementary Tools

- **[Google Hacking Database (GHDB)](https://www.exploit-db.com/google-hacking-database)**: A public repository of common Google Dorks.
- **[Shodan](https://www.shodan.io/)**: A tool for identifying devices connected to the internet.
- **[FOCA](https://www.elevenpaths.com/labstools/foca)**: A tool for metadata analysis.

---

## ⚠️ Legal Disclaimer

This content is intended for educational purposes only and must be used within the bounds of the law. Misuse of these techniques may violate local or international laws. Please be responsible!

---

## 📚 Additional Resources

- [Google's Official Search Operators Guide](https://support.google.com/websearch/answer/136861)
- [OWASP Internet Security Documentation](https://owasp.org/)
- [Exploit-DB](https://www.exploit-db.com/)

---

## 🖊 Contributions

Have suggestions or want to add more content? Feel free to open an issue or submit a pull request

---
