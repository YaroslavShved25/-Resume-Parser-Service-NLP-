

# 📄 Resume Parser Service (GPT-3 Powered)

A **GPT-3 based Resume Parser REST API** that converts resume PDFs into clean, structured JSON files.  
This service accurately extracts key fields such as contact information, education, job experience, and project history.

Example:
- 📄 [Input PDF](https://github.com/YaroslavShved25/-Resume-Parser-Service-NLP-/examples/SDE_May2023_HuanXu.pdf)
- 🗂️ [Parsed JSON Output](https://github.com/YaroslavShved25/-Resume-Parser-Service-NLP-/examples/resume.json)

---

## 🚀 Features
- ✅ Fast and accurate resume parsing using GPT-3 (`text-davinci-002`)
- ✅ JSON response ready for ATS and HR system integration
- ✅ Supports most common resume formats
- ✅ Flask-powered REST API for easy deployment
- ✅ Environment-based OpenAI key management

---

## 💰 Token Usage & Cost
Parsing a resume typically takes **~15 seconds** and consumes:
- ~1500 tokens (~$0.03)
- Larger resumes may consume up to ~3000 tokens (~$0.06)

*(Based on OpenAI’s pricing model for the `text-davinci-002` engine.)*

⚡ **Fine-tuning GPT-3 could further improve accuracy, but out-of-the-box performance is already excellent.**

---

## ⚙️ Quick Start

### 1. Install Prerequisites
- Python 3.7+
- `pip3`


*(For macOS users, see additional instructions below.)*

### 2. Setup
```bash
git clone https://github.com/YaroslavShved25/-Resume-Parser-Service-NLP-.git
cd resume-parser-service

# Upgrade pip if needed
python3 -m pip install --upgrade pip
````

### 3. Build the Project

```bash
./build.sh
```

### 4. Set Your OpenAI API Key

* Create a `.env` file:

```text
OPENAI_API_KEY=YOUR_API_KEY
```

OR

* Set it as an environment variable:

```bash
export OPENAI_API_KEY=YOUR_API_KEY
```

### 5. Run the Service

```bash
./run.sh
```

Access the API: [http://0.0.0.0:5001/](http://0.0.0.0:5001/)

---

### 🖥️ macOS Setup Notes

You must install:

* Xcode (run it at least once to complete setup)
* Command Line Tools:

```bash
xcode-select --install
```

* [Homebrew](https://brew.sh/)
* Python 3 via:

```bash
brew install python
```

---

## 📂 Supported Fields

### 🎯 Basic Information

* First Name
* Last Name
* Full Name
* Email
* U.S. Phone Number
* Location
* Portfolio Website URL
* LinkedIn URL
* GitHub URL

### 🎓 Education

* University
* Degree Level
* Graduation Year & Month
* Majors
* GPA

### 💼 Job Experience

* Job Title
* Company
* Location
* Duration
* Job Description

### 🛠️ Project Experience

* Project Name
* Project Description

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙋‍♂️ Questions or Contributions?

Feel free to reach out or open an issue.
Pull requests are welcome!

```


