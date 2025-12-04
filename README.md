# building-a-version-control-system
# 🚀 Version Control System (VCS) — README

Welcome to the **Version Control System (VCS)** project! This README explains everything about your custom VCS — what it does, how it works, how to install, and how to use it.

---

## 📌 Overview

This project is a simple, beginner‑friendly **Version Control System** similar to Git but built from scratch for learning purposes.

It helps you:

* Track file changes
* Commit and store versions
* View commit history
* Restore old versions
* Manage repository structure

---

## 🛠 Features

* 📂 Initialize repository (`vcs init`)
* ➕ Add files (`vcs add <filename>`)
* 💾 Commit changes (`vcs commit -m "message"`)
* 📜 View history (`vcs log`)
* 🔄 Restore version (`vcs checkout <commit_id>`)
* 🧹 Clean and organize metadata folder

Everything is stored inside a hidden folder named `.vcs/`.

---

## 📁 Project Structure

```
project-directory/
│
├── .vcs/
│   ├── commits/
│   ├── index/
│   ├── HEAD
│   └── log
│
├── your source files...
└── vcs.py
```

---

## ⚙️ Installation

Clone or download this project and ensure you have **Python 3.8+**.

```bash
git clone <your-repo-url>
cd vcs-project
python vcs.py
```

Or run commands directly:

```bash
python vcs.py init
```

---

## 🚀 Usage

Below are all available commands.

### **1️⃣ Initialize a Repository**

```bash
python vcs.py init
```

Creates `.vcs/` folder.

---

### **2️⃣ Add Files to Staging**

```bash
python vcs.py add file.txt
```

Copies file to staging area.

---

### **3️⃣ Commit Changes**

```bash
python vcs.py commit -m "your message"
```

Creates snapshot and stores version.

---

### **4️⃣ View Commit History**

```bash
python vcs.py log
```

Shows commit ID, timestamp, and message.

---

### **5️⃣ Restore a Commit**

```bash
python vcs.py checkout <commit_id>
```

Restores file versions from old commit.

---

## 🧠 Internal Working

### **1. Staging Area**

Files added via `vcs add` go into `.vcs/index/`.

### **2. Committing**

When committing:

* A unique commit ID is generated
* Staged files are copied into `.vcs/commits/<commit-id>/`
* A log entry is saved

### **3. Checkout**

Restores project files from selected commit folder.

---

## 🛡️ Error Handling

The system shows friendly errors:

* Repository not initialized
* Nothing to commit
* File not found
* Commit ID does not exist

---

## 📌 Future Improvements

* Branching system
* Merge functionality
* Remote push/pull support
* Diff viewer

---

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit PRs.

---

## 📄 License

This project uses the **MIT License**. You can modify and use it freely.

---


