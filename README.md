# Dynamic Data Handling with Data Attributes - JavaScript Project #1

This project demonstrates dynamic data handling using JavaScript and data attributes. It features a responsive card-based UI and models for detailed profile viewing, accompanied by animations and confetti effects for an engaging user experience.

---

## 🛠️ Features

- **Dynamic Data Access:** Fetch profile details dynamically using JavaScript and data attributes.
- **Interactive UI:** Responsive card design with modals for detailed profile information.
- **Animations:** Smooth animations using GSAP for an interactive experience.
- **Confetti Effect:** Fun confetti effects are triggered on the profile view.
- **User-Friendly Design:** Clean and modern card-based layout.

---

## 🎥 Demo

![Demo](assets/demo.gif)  

---

## 🖼️ UI Preview

### Card View  
The main view consists of visually appealing cards representing user profiles.

![Card UI](assets/card%201.png)  

---

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/Shehryar-dev/Dynamic-Data-Handling---JavaScript-Project-1.git
   ```
2. Open the `index.html` file in your browser to explore the project.

---

## 📄 Code Highlights

### JavaScript Functionality

#### Dynamic Data Access
The data attributes (`data-name`, `data-age`, `data-company`, `data-img`) are accessed and displayed dynamically in the modal using JavaScript. Here's an example:

```javascript
function showProfile() {
    const profile = document.querySelector("#name-3").parentNode;
    const name = profile.querySelector("[data-name]").getAttribute("data-name");
    document.getElementById("name-3").innerHTML = name;
}
```

#### Confetti Effect
Confetti animations are added using the `confetti` library for a celebratory effect.

```javascript
confetti({
    angle: randomInRange(55, 125),
    spread: randomInRange(50, 70),
    particleCount: randomInRange(50, 100),
    origin: { y: 0.6 }
});
```

#### GSAP Animations
Smooth animations for cards and the body.

```javascript
gsap.from('div.col-B', { duration: 2, x: "150%", opacity: 1, ease: "power2.in", delay: 1 });
```

---

## 💻 Technologies Used

- **HTML5**: Markup for the structure.
- **CSS3**: Styling for the card-based UI and modal.
- **JavaScript**: Core functionality for data access and dynamic rendering.
- **GSAP**: For animations.
- **Confetti.js**: To add confetti effects.

---

## 🌟 Customization

- **Add New Profiles:** Update the HTML with new cards and assign appropriate `data-*` attributes.
- **Styling Adjustments:** Modify the CSS to suit your design preferences.
- **Animations:** Enhance or change animations using GSAP.

---

### ✨ Credits
Designed and developed by **@Shehryar-dev**.  
If you like this project, give it a ⭐ on GitHub!

---

## 💼 Connect

- **LinkedIn**: [LinkedIn](https://www.linkedin.com/in/shehryarkhandiv)
- **GitHub**: [GitHub](https://github.com/Shehryar-dev)
- **Twitter**: [X Account](https://x.com/Morphues_S)
- **Portfolio**: [Portfolio](https://shehriyar-portfolio-v2.netlify.app/)
