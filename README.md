# 📧 JavaFX Email Client

A modern, feature-rich desktop email client built with <img src="https://img.shields.io/badge/Java-ED8B00?style=flat&logo=java&logoColor=white" height="20"/> and <img src="https://img.shields.io/badge/JavaFX-1B6AC6?style=flat&logo=java&logoColor=white" height="20"/>. Supports multiple accounts, persistent login, email sending/receiving, attachments, and a customizable user interface.

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Desktop-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  
</p>

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" height="28"/>
  <img src="https://img.shields.io/badge/JavaFX-3776AB?style=for-the-badge&logo=javafx&logoColor=white" height="28"/>
  <img src="https://img.shields.io/badge/JavaMail-007396?style=for-the-badge&logo=mailchimp&logoColor=white" height="28"/>
  <img src="https://img.shields.io/badge/FXML-3776AB?style=for-the-badge&logo=xml&logoColor=white" height="28"/>
  <img src="https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white" height="28"/>
</p>


- **Java 11+** <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" width="22"/>
- **JavaFX** (UI, FXML, CSS) <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/javafx-original.svg" width="22"/>
- **JavaMail API** (IMAP/SMTP)
- **MVC Pattern**
- **Multi-threading** (JavaFX Services/Tasks)
- **Serialization** (Persistence)

---

## 🚀 Features

- <img src="https://img.icons8.com/fluency/24/000000/multiple-users.png"/> **Multi-Account Support**: Add, remove, and switch between multiple email accounts.
- <img src="https://img.icons8.com/fluency/24/000000/lock-2.png"/> **Persistent Login**: Securely saves credentials  for seamless startup.
- <img src="https://img.icons8.com/fluency/24/000000/inbox.png"/> **Inbox Management**: Browse folders, view messages, mark as read/unread, delete, and view details.
- <img src="https://img.icons8.com/fluency/24/000000/compose.png"/> **Compose & Send Emails**: Rich text editor, attachments, select sender account.
- <img src="https://img.icons8.com/fluency/24/000000/attach.png"/> **Attachments**: Attach files to outgoing emails, download and open received attachments.
- <img src="https://img.icons8.com/fluency/24/000000/paint-palette.png"/> **Customizable UI**: Switch between light/dark/default themes and multiple font sizes.
- <img src="https://img.icons8.com/fluency/24/000000/rocket.png"/> **Responsive & Fast**: All network operations run in the background for a smooth experience.
- <img src="https://img.icons8.com/fluency/24/000000/flow-chart.png"/> **MVC Architecture**: Clean separation of concerns for maintainability and extensibility.

---



## 🖥️ Screenshots

### 🔐 Login
<p align="center">
 
  <img src="https://github.com/Elaf24/EmailClient/assets/110555263/7f2889f6-acc1-438d-b1f7-42111dbee10b" alt="Main Window" width="600"/>
</p>

### 📥 Inbox View
<p align="center">
  <img src="https://github.com/Elaf24/EmailClient/assets/110555263/5af22d5f-1679-4628-a768-13f9701ddb82" alt="Compose Email" width="600"/>
</p>

### ✉️ Email Drafting View
<p align="center">
   <img src="https://github.com/Elaf24/EmailClient/assets/110555263/acab9dd1-537b-4780-a1e0-c2422cf31f4d" alt="Options Window" width="600"/>
</p>

### ⚙️ Settings Menu
<p align="center">
  
  <img src="https://github.com/Elaf24/EmailClient/assets/110555263/727facbe-e6dd-48d9-aa6b-f34e81df4dcf" alt="Login Window" width="600"/>
</p>


---

## 🏗️ Architecture

- <img src="https://img.icons8.com/color/24/000000/java-coffee-cup-logo.png"/> **Language:** Java
- <img src="https://img.icons8.com/color/24/000000/javafx.png"/> **UI:** JavaFX (FXML, CSS)
- <img src="https://img.icons8.com/ios-filled/24/000000/flow-chart.png"/> **Pattern:** Model-View-Controller (MVC)
- <img src="https://img.icons8.com/fluency/24/000000/mail.png"/> **Email Protocols:** IMAP (receive), SMTP (send) via JavaMail API
- <img src="https://img.icons8.com/fluency/24/000000/save-close.png"/> **Persistence:** Serializable file with encoded credentials
- <img src="https://img.icons8.com/fluency/24/000000/multiple-processes.png"/> **Multi-threading:** JavaFX Services/Tasks for background operations

---

## 📂 Project Structure

```
EmailClient-JAVA-main/
├── src/
│   └── com/Project/
│       ├── controller/         # UI controllers (Login, Main, Compose, Options, Details)
│       ├── model/              # Data models (EmailAccount, EmailMessage, etc.)
│       ├── view/               # FXML layouts, CSS themes, icons
│       ├── EmailManager.java   # Core logic for managing accounts, folders, messages
│       └── Launcher.java       # Application entry point
│
├── README.md
└── ...
```

---

## ⚙️ Setup & Running

### **Requirements**

- <img src="https://img.icons8.com/color/20/000000/java-coffee-cup-logo.png"/> Java 11 or higher
- <img src="https://img.icons8.com/color/20/000000/javafx.png"/> JavaFX SDK
- <img src="https://img.icons8.com/fluency/20/000000/mail.png"/> JavaMail API (included in dependencies)

### **Run from IDE (IntelliJ/Eclipse):**

1. Clone the repository.
2. Import as a Maven/Gradle/Java project.
3. Ensure JavaFX and JavaMail libraries are configured.
4. Run `com.Project.Launcher`.

### **Run from Command Line:**

```sh
javac -d out src/com/Project/**/*.java
java -cp out com.Project.Launcher
```

---

## 🛠️ Main Components

| <img src="https://img.icons8.com/ios-filled/20/000000/module.png"/> Component | <img src="https://img.icons8.com/ios-filled/20/000000/info.png"/> Description |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `Launcher.java`                                                               | Application entry, loads/saves accounts, shows main/login window              |
| `EmailManager.java`                                                           | Core logic for accounts, folders, messages                                    |
| `controller/`                                                                 | UI logic for each window (login, main, compose, options, details)             |
| `model/`                                                                      | Data models: EmailAccount, EmailMessage, etc.                                 |
| `view/`                                                                       | FXML layouts, CSS themes, icons                                               |
| `services/`                                                                   | Background tasks: login, fetch, send, render                                  |
| `persistence/`                                                                | Account storage, encoding/decoding credentials                                |

---

## 🎨 Customization

- <img src="https://img.icons8.com/fluency/20/000000/paint-palette.png"/> **Themes:** Switch between light, dark, and default themes in the Options window.
- <img src="https://img.icons8.com/fluency/20/000000/font-size.png"/> **Font Size:** Choose from small, medium, or large fonts.
- <img src="https://img.icons8.com/fluency/20/000000/icons8-css3.png"/> **Icons & CSS:** Easily replace icons or tweak CSS in `src/com/Project/view/css/`.

---

## 🧩 Technologies & Concepts

- <img src="https://img.icons8.com/color/20/000000/javafx.png"/> **JavaFX:** FXML, CSS, custom nodes, TableView, WebView
- <img src="https://img.icons8.com/fluency/20/000000/mail.png"/> **JavaMail:** IMAP/SMTP, message parsing, attachments
- <img src="https://img.icons8.com/fluency/20/000000/multiple-processes.png"/> **Multi-threading:** JavaFX Services/Tasks
- <img src="https://img.icons8.com/fluency/20/000000/save-close.png"/> **Persistence:** Serialization, encoding
- <img src="https://img.icons8.com/ios-filled/20/000000/flow-chart.png"/> **MVC Pattern**

---

## 📬 Email Features

- <img src="https://img.icons8.com/fluency/20/000000/lock-2.png"/> **Login:** Secure authentication with IMAP/SMTP
- <img src="https://img.icons8.com/fluency/20/000000/inbox.png"/> **Inbox:** Browse folders, view messages, mark read/unread, delete
- <img src="https://img.icons8.com/fluency/20/000000/compose.png"/> **Compose:** Rich text, attachments, select sender
- <img src="https://img.icons8.com/fluency/20/000000/attach.png"/> **Attachments:** Add, download, open
- <img src="https://img.icons8.com/fluency/20/000000/details-pane.png"/> **Details:** View full message, sender, subject, attachments

---

## ❓ FAQ

**Q: Where are my credentials stored?**  
A: In a serialized file in your home directory, with passwords encoded for basic security.

**Q: Can I use this with Gmail, Outlook, etc.?**  
A: Yes, as long as IMAP/SMTP is enabled and you use an app password if required.

**Q: How do I change the theme or font size?**  
A: Go to the Options window from the Edit menu.

---

## 🤝 Contributing

Pull requests and suggestions are welcome! Please open an issue to discuss changes or improvements.

---

## 📄 License

This project is licensed under the MIT License.
