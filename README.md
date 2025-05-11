Here's a basic `README.md` file tailored for your Flask Contact Form application, including key features, technologies used, and setup instructions:

---

### 📄 `README.md`

```markdown
# 📬 Flask Contact Form Application

This is a web-based contact form built using Python and Flask. It allows users to submit their name, email, subject, message, and optionally upload a file. Submissions are saved to a SQLite database and email notifications are sent to both the admin and the user.

---

## 🚀 Features

- Contact form with file upload (supports JPG, PNG, PDF, DOCX)
- Google reCAPTCHA integration for spam prevention
- Email notifications using Gmail SMTP (Flask-Mail)
- Admin login and dashboard to view submissions
- Data stored in a local SQLite database

---

## 🛠️ Technologies Used

- Python 3
- Flask
- SQLite
- Flask-Mail
- Google reCAPTCHA
- HTML/CSS/JavaScript

---

## 📁 Project Structure

```

project-root/
│
├── static/
│   ├── style.css
│   └── script.js
│
├── templates/
│   ├── ContactForm.html
│   ├── admin\_login.html
│   ├── admin\_dashboard.html
│   └── 500.html
│
├── uploads/                # Uploaded files will be stored here
├── contact.db              # SQLite database
├── app.py                  # Main Flask application
└── README.md

````

---

## ⚙️ Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/flask-contact-form.git
   cd flask-contact-form
````

2. **Create a virtual environment (optional but recommended):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Update Gmail SMTP credentials:**
   Edit `app.py`:

   ```python
   app.config.update(
       MAIL_USERNAME='your-email@gmail.com',
       MAIL_PASSWORD='your-app-password'
   )
   ```

5. **Enable Google reCAPTCHA v2** and replace the `sitekey` and `secret` in `ContactForm.html` and `app.py`.

6. **Run the app:**

   ```bash
   python app.py
   ```

7. **Access the app:**
   Visit `http://localhost:5000`

---

## 🔒 Admin Login

Default admin credentials:

* Username: `syam`
* Password: `syam2003`

> Change these in `app.py` for better security.

---

## 📧 Contact

For issues or feature requests, please open an [issue](https://github.com/yourusername/flask-contact-form/issues) on GitHub.

```

---

Would you like me to create a `requirements.txt` file next?
```
