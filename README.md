# 🛡️ Overwatch 2 Fan Page - Heroes Never Die

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Deployment](https://img.shields.io/badge/Deployed%20on-AWS%20S3-FF9900?logo=amazonaws)
![License](https://img.shields.io/badge/License-MIT-blue)

> A modern, responsive landing page dedicated to the Overwatch 2 universe, deployed on AWS cloud infrastructure.

[**🌐 VIEW LIVE DEMO**](http://your-domain-here.com) ## 📖 Project Overview

This project is a static website developed to demonstrate modern frontend layout skills and cloud deployment workflows. The interface features a "Dark Mode" aesthetic inspired by Overwatch 2, utilizing geometric typography and a vibrant color palette.

Beyond the design, the core objective of this project was to **implement a real-world cloud deployment strategy** using an Amazon S3 Bucket configured for static hosting, connected to a custom domain provided by the GitHub Student Developer Pack.

## 🚀 Tech Stack

### Frontend
* **HTML5:** Semantic structure.
* **CSS3:**
    * **Flexbox & Grid:** Used for the character roster layout and responsive navigation.
    * **CSS Variables:** Efficient color management (`--primary`, `--bg-dark`).
    * **Media Queries:** Fully responsive design (Mobile First approach).
    * **Animations:** Smooth transitions and hover effects on cards and buttons.
* **FontAwesome:** Iconography for social media and the hamburger menu.

### Infrastructure & Deployment
* **AWS S3:** Static website hosting (Bucket Policies & Public Access configuration).
* **DNS Management:** CNAME/A Record configuration to point the custom domain to the AWS S3 endpoint.
* **Git & GitHub:** Version control.

## 📸 Project Gallery

Here are some screenshots of the application running on different devices:

### 🖥️ Desktop View
_Home landing page featuring the Hero Section and transparent navigation._
![Desktop Preview](./screenshots/desktop-preview.png)

### 📱 Mobile View (Responsive)
_Responsive character grid adaptation and functional hamburger menu without JavaScript._
<p float="left">
  <img src="./screenshots/mobile-view.png" width="45%" />
  <img src="./screenshots/menu-mobile.png" width="45%" /> 
</p>

## 🎨 Design Features

* **Pure CSS Navigation:** A fully functional hamburger menu implemented using the "Checkbox Hack" (`<input type="checkbox">`), avoiding JavaScript to keep the site lightweight.
* **Responsive Roster Grid:** Utilizes `grid-template-columns: repeat(auto-fit, minmax(...))` to automatically adjust character cards based on the screen width.
* **Gaming Aesthetic:** Dark gradients, neon shadows, and italicized typography to replicate the game's UI feel.

## 🔧 Installation & Local Use

If you want to clone this project to view it locally:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR-USERNAME/YOUR-REPO.git](https://github.com/YOUR-USERNAME/YOUR-REPO.git)
    ```
2.  **Navigate to the folder:**
    ```bash
    cd YOUR-REPO
    ```
3.  **Run:**
    Simply open the `index.html` file in your preferred browser or use the "Live Server" extension in VS Code.

## ☁️ Deployment Details (AWS S3)

The site is hosted on an **S3 Bucket** with "Static website hosting" enabled.

1.  **Public Access:** A Bucket Policy was configured to allow public read access (`s3:GetObject`).
2.  **Domain Mapping:** The custom domain DNS records were updated to point to the S3 website endpoint.

## 👤 Author

**Your Name**
* **Portfolio:** [Link to your Portfolio]
* **LinkedIn:** [Link to your LinkedIn]
* **GitHub:** [@YourUsername](https://github.com/YourUsername)

---
*This project is a Fan Page created for educational purposes. All image rights and characters belong to Blizzard Entertainment.*
