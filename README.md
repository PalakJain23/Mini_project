# Mini_project
Mini project front_end development

<!-- <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mini project</title>
    <link rel="stylesheet" href="miniproject.css77" />
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Manufacturing+Consent&family=Roboto:ital,wght@0,100..900;1,100..900&display=swap" 
    rel="stylesheet">
    <link rel="stylesheet" 
    href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200&icon_names=home" />
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200&icon_names=check_circle" />

</head>
<body>
    <h1>Apna college </h1>
    <span class="material-symbols-outlined">
    
home
</span>
<span class="material-symbols-outlined">
check_circle
</span>
</body>
</html> -->

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


css code 
/* Reset default browser styles and set font */
* {
  margin: 0;
  padding: 0;
  font-family: "Roboto", sans-serif;
  box-sizing: border-box;
}

/* Background area with full screen height and background image */
.main_box {
  background: url("photo.jpg") no-repeat center center/cover; /* covers entire box */
  height: 100vh; /* full screen height */
  position: relative; /* required for absolute positioning of button */
}

/* Open (hamburger) button style */
.btn_one {
  color: white;
  font-size: 30px;
  font-weight: bold;
  position: absolute;
  left: 16px;
  line-height: 60px;
  cursor: pointer;
  z-index: 2; /* stays above the sidebar */
}

/* Sidebar menu styling (hidden initially) */
.sidebar_menu {
  position: fixed;
  top: 0;
  left: -300px; /* hides the sidebar to the left */
  height: 100vh;
  width: 300px;
  background-color: rgba(255, 255, 255, 0.1); /* semi-transparent white */
  box-shadow: 0 2px 6px rgba(255, 255, 255, 0.5);
  transition: all 0.3s ease; /* smooth slide-in effect */
  z-index: 1;
}

/* Sidebar logo area */
.sidebar_menu .logo {
  width: 100%;
  line-height: 60px;
  box-shadow: 0 0 4px rgba(255, 255, 255, 0.5);
  text-align: center;
}

/* Logo text link */
.sidebar_menu .logo a {
  color: white;
  text-decoration: none;
  font-size: 20px;
  font-weight: 500;
}

/* Sidebar menu list styling */
.sidebar_menu .menu {
  width: 100%;
  margin-top: 20px;
  list-style: none; /* removes bullet points */
}

/* Each list item in the sidebar */
.sidebar_menu .menu li {
  margin-top: 6px;
  padding: 14px 20px;
}

/* Icon and text inside each menu item */
.sidebar_menu .menu li i,
.sidebar_menu .menu li a {
  text-decoration: none;
  color: white;
}

/* Spacing between icon and text */
.sidebar_menu .menu li i {
  padding-right: 8px;
}

/* Hover effect for menu items */
.sidebar_menu .menu li:hover {
  box-shadow: 0 0 4px rgba(255, 255, 255, 0.5);
}

/* Close (X) button style */
.sidebar_menu .btn_two {
  color: grey;
  font-size: 30px;
  font-weight: bold;
  position: absolute;
  left: 275px;
  top: 10px;
  cursor: pointer;
}

/* Social media icons container at bottom */
.sidebar_menu .social_media {
  position: absolute;
  left: 25%;
  bottom: 50px;
  display: flex;
  gap: 10px; /* spacing between icons */
}

/* Individual social media icons */
.sidebar_menu .social_media i {
  color: white;
  opacity: 0.5;
  transition: 0.3s ease;
}

/* Hover effect on social media icons */
.sidebar_menu .social_media i:hover {
  opacity: 1;
  transform: scale(1.1);
}

/* Hover effect on menu buttons */
.btn_one:hover i,
.btn_two:hover i {
  font-size: 35px;
}

/* Hides the checkbox input used to toggle the sidebar */
#check {
  display: none;
}

/* When checkbox is checked, move sidebar to visible */
#check:checked ~ .sidebar_menu {
  left: 0; /* show the sidebar */
}

#check:checked ~ .btn_one i{
  opacity: 0;
}

#check:checked ~ .sidebar_menu .btn_two i{
  opacity: 1;
}

