# Mini_project
Mini project front_end development

# Sidebar Menu Project

This is a responsive sidebar navigation menu built using **HTML** and **CSS**. It includes a slide-in sidebar with a toggle (hamburger) button, close button, logo section, menu items, and social media icons.

---

## 📸 Preview

![screenshot](menu.jpg)

---

## 🛠️ Features

- Full-screen background with image
- Sliding sidebar using CSS only (checkbox trick)
- Logo and navigation menu
- Social media icons with hover effects
- Smooth transition animations
- Responsive layout

---

## 📂 File Structure

project-folder/
│
├── index.html # Main HTML file
├── style.css # CSS file for styling
├── photo.jpg # Background image
└── README.md # Project documentation

## 💡 How It Works

- A hidden `<input type="checkbox" id="check">` is used to control the sidebar visibility.
- The `.btn_one` (hamburger icon) is linked to the checkbox.
- When checked, the sidebar (`.sidebar_menu`) slides in using CSS transition.
- `.btn_two` is used to close the sidebar by unchecking the checkbox.
- The layout is fully handled using **pure HTML & CSS**, without JavaScript.

---

## 🧪 How to Use

1. Clone or download the project.
2. Place an image named `photo.jpg` in the same folder as `index.html`.
3. Open `index.html` in a browser.

---

## 🖌️ Customization Tips

- Change background image in `.main_box` (CSS).
- Modify sidebar color by editing `.sidebar_menu`.
- Add/remove menu items as needed inside the `<ul class="menu">`.
- Replace Font Awesome icons or text to suit your project.

---

## 🧾 License

This project is open-source and free to use for educational and personal projects.

---

## 🙋‍♀️ Author

**Palak Jain**  
Second-year AI student  
🧠 Passionate about web development and machine learning


<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Project</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins&display=swap"
      rel="stylesheet"
    />
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"
    />
    <link href="https://fonts.googleapis.com/css2?family=Libertinus+Mono&family=Manufacturing+Consent&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="miniproject.css">
  </head>
  <body>
    <div class="main_box">
      <input type="checkbox" id="check" />
      <div class="btn_one">
        <label for="check">
          <i class="fa-solid fa-bars"></i>
        </label>
      </div>

      <div class="sidebar_menu">
        <div class="logo">
          <a href="#">Apna College</a>
        </div>

        <div class="btn_two">
          <label for="check" >
            <i class="fa-solid fa-xmark"></i>
          </label>
        </div>

        <div class="menu">
          <ul>
            <li>
              <i class="fa-solid fa-image"></i>
              <a href="#">Gallery</a>
            </li>
            <li>
              <i class="fa-solid fa-arrow-up-right-from-square"></i>
              <a href="#">Shortcuts</a>
            </li>
            <li>
              <i class="fa-solid fa-photo-film"></i>
              <a href="#">Exhibits</a>
            </li>
            <li>
              <i class="fa-solid fa-calendar-days"></i>
              <a href="#">Events</a>
            </li>
            <li>
              <i class="fa-solid fa-store"></i>
              <a href="#">Store</a>
            </li>
            <li>
              <i class="fa-solid fa-phone"></i>
              <a href="#">Contact</a>
            </li>
            <li>
              <i class="fa-regular fa-comments"></i>
              <a href="#">Feedback</a>
            </li>
          </ul>
        </div>

        <div class="social_media">
          <ul>
            <a href="#"><i class="fa-brands fa-facebook"></i></i></a>
            <a href="#"><i class="fa-brands fa-twitter"></i></a>
            <a href="#"><i class="fa-brands fa-instagram"></i></i></a>
            <a href="#"><i class="fa-brands fa-youtube"></i></a>
          </ul>
        </div>
      </div>
    </div>
  </body>
</html>


