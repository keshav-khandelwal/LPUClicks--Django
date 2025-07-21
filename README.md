# 📸 LPU Clicks – A Social Media Platform for LPU Students

LPU Clicks is a dynamic, full-stack social media platform created exclusively for the students of **Lovely Professional University (LPU)** to share their campus life through photos, events, and experiences.

The platform aims to foster a vibrant community where students can **capture moments**, **connect with peers**, and **participate in trending campus challenges**.

---

## 🌟 Features

### 🎨 UI/UX & Branding
- **Modern, responsive UI** built with **Bootstrap 5**, **custom CSS**, and **Google Fonts (Poppins)**.
- Theme inspired by LPU's official branding:
  - **Primary color**: Orange `#f7931e`
  - **Accent**: Black and White
- Clean layouts with animated search, modals, and smooth user interactions.

### 👥 User Authentication
- User registration and login system.
- Profile creation and editing with image upload.

### 🖼️ Post Feed
- A central feed showing uploaded **images with captions**, likes, and user details.
- Responsive layout with Bootstrap cards and Font Awesome icons.

### 📂 Media Management
- Upload, display, and manage:
  - Profile pictures
  - Post images
- Images stored in `/media/profile_images/` and `/media/post_images/`.

### 🔍 Advanced Search
- Real-time **user search modal** with animation and search result cards.
- Custom-designed cards displaying matching usernames and profile pictures.

### 🔧 Admin Features (WIP)
- Admin panel to manage users and posts.
- Reporting and moderation features coming soon.

---

## 🛠 Tech Stack

| Layer       | Technologies Used                                     |
|-------------|--------------------------------------------------------|
| Frontend    | HTML5, CSS3, Bootstrap 5, JavaScript, Tailwind (planned) |
| Backend     | Django 5.2.4                                           |
| Database    | SQLite (local), PostgreSQL on Render (for production) |
| Deployment  | **Render** platform for backend hosting               |
| Media Files | Django media file system                              |
| Fonts & Icons | Google Fonts (Poppins), Font Awesome               |

---

## 🧑‍💻 Project Structure

```
LPUClicks--Django/
│
├── media/                     # Uploaded images
│   ├── post_images/
│   └── profile_images/
│
├── static/                    # Static CSS/JS files
│
├── templates/                 # HTML templates
│   ├── feed.html
│   ├── profile.html
│   ├── edit_profile.html
│   ├── explore.html
│   └── search_results.html
│
├── lpuclicks/                 # Django project files
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── user/                      # Main app: handles models, views, forms
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── forms.py
│   └── templates/
│
└── manage.py
```

---

## 🚀 How to Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/keshav-khandelwal/LPUClicks--Django
   cd LPUClicks--Django
   ```

2. **Create Virtual Environment**
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply Migrations & Run Server**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   python manage.py runserver
   ```

5. **Open in Browser**
   ```
   http://127.0.0.1:8000/
   ```

---

## 🌐 Deployment (Render)

- Hosted on: `https://lpuclicks.onrender.com/`
- Set environment variables:
  - `SECRET_KEY`
  - `DEBUG=False`
  - `ALLOWED_HOSTS=['lpuclicks.onrender.com']`
- Setup PostgreSQL via Render and connect it in `settings.py`.

---

## 🧩 Future Features

- 📷 **Video Upload Support**
- 📌 **Hashtag-based Post Filters**
- 📊 **Analytics Dashboard for Admins**
- 🔔 **Real-time Notifications (via Channels)**
- 💬 **Comment & Chat System**

---

## 👨‍💻 Developer Info

- **Name:** Keshav Khandelwal
- **Role:** Full Stack Developer
- **University:** Lovely Professional University (B.Tech CSE)
- **Connect:**
  - [GitHub](https://github.com/keshav-khandelwal)
  - [LinkedIn](https://www.linkedin.com/in/keshav-khandelwal-kk/)
  - 📧 Email: keshavkhandelwal.me@gmail.com

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).

---

## ❤️ Acknowledgments

- Special thanks to LPU community and friends for design inspiration.
- Bootstrap, Django, Font Awesome, and open-source contributors.
