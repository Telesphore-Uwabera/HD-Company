# HD Company

```markdown
## HD-Company - Revitalizing Web Design

HD-Company is a project aimed at revitalizing web design through a Bootstrap 5-based recreation of a one-page website, inspired by the Braintech Technology IT Solutions HTML Template. The project focuses on refining Bootstrap 5 skills and enhancing HTML/CSS proficiency by customizing the template.

### Project Structure

```plaintext
HD-Company/
├── index.html
├── css/
│   └── styles.css
├── js/
│   └── scripts.js
└── assets/
    ├── images/
    └── fonts/
```

### Setup Instructions

To run this project locally:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/Telesphore-Uwabera/HD-Company.git
   ```

2. Open `index.html` in your web browser.

### Customizations

- **Color Scheme**: Tailored to complement the chosen theme.
- **Content**: Replaced placeholder text and images with relevant content.
- **Enhancements**: Implemented smooth scrolling for navigation links using JavaScript.

### Key Styling Features

Custom CSS (`styles.css`) significantly enhances the website's design and user experience:

#### General Styles

- **Font and Scroll Behavior**: Utilizes 'Roboto' font for a modern look and smooth scrolling for seamless navigation.
- **Navbar**: Customized brand appearance and link colors for improved aesthetics and usability.

#### Hero Section

- **Visual Appeal**: Centered background image and text for a compelling introduction.

#### Services Section

- **Interactive Cards**: Added hover effects to engage users with service details.

#### About Section

- **Text Readability**: Improved legibility through enhanced font size and spacing.

#### Portfolio Section

- **Highlighted Images**: Applied hover effects to showcase portfolio items effectively.

#### Team Section

- **Engaging Cards**: Hover effects maintain consistency and user interaction.

#### Contact Section

- **Form Usability**: Bold labels enhance form clarity and user experience.

#### Footer

- **Clean Layout**: Enhanced padding and alignment for a polished appearance.

#### Back to Top Button

- **User Navigation**: Fixed-position button with hover effects for convenient page scrolling.

### JavaScript Enhancements

#### Smooth Scrolling

```javascript
document.querySelectorAll('a.nav-link').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const targetSection = document.querySelector(this.getAttribute('href'));
        targetSection.scrollIntoView({
            behavior: 'smooth',
            block: 'start'
        });
    });
});
```

#### Back to Top Button

```javascript
const backToTopButton = document.createElement('button');
backToTopButton.innerText = 'Top';
backToTopButton.className = 'btn btn-primary back-to-top';
document.body.appendChild(backToTopButton);

backToTopButton.style.position = 'fixed';
backToTopButton.style.bottom = '20px';
backToTopButton.style.right = '20px';
backToTopButton.style.display = 'none';

window.addEventListener('scroll', () => {
    if (window.scrollY > 300) {
        backToTopButton.style.display = 'block';
    } else {
        backToTopButton.style.display = 'none';
    }
});

backToTopButton.addEventListener('click', () => {
    window.scrollTo({
        top: 0,
        behavior: 'smooth'
    });
});
```

### Technologies Used

- **Bootstrap 5**: Front-end framework for responsive design.
- **HTML5**: Structure and content of web pages.
- **CSS3**: Styling and customization.
- **JavaScript**: Enhancing interactivity.

### Contributors

- [Telesphore Uwabera](https://github.com/Telesphore-Uwabera)

### License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Visit the HD-Company website [here](https://telesphore-uwabera.github.io/HD-Company/).
```
