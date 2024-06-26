```markdown
## HD-Company

This project replicates a one-page website using Bootstrap 5, based on the Braintech Technology IT Solutions HTML Template. It aims to enhance Bootstrap 5 skills for responsive design and improve HTML/CSS proficiency by customizing the template.

## Project Structure

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

## Setup Instructions

To run this project locally:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/Telesphore-Uwabera/HD-Company.git
   ```

2. Open `index.html` in your web browser.

## Customizations Made

- **Color Scheme**: Customized to match the chosen theme.
- **Content**: Replaced placeholder content with relevant information and images.
- **Additional Features**: Implemented smooth scrolling for navigation links using JavaScript.

## Custom Styling Significance

The custom CSS in `styles.css` plays a crucial role in enhancing the design and user experience of the website. Key aspects include:

### General Styles

- **Font and Scroll Behavior**: Set the font to 'Roboto' and implemented smooth scrolling for navigation.
- **Navbar**: Customized navbar brand and link colors for improved visibility.

### Hero Section

- **Background and Text Alignment**: Centered background image and text for visual appeal.

### Services Section

- **Card Hover Effect**: Added hover effect for interactive user experience.

### About Section

- **Text Styling**: Enhanced readability with increased font size and line height.

### Portfolio Section

- **Image Hover Effect**: Highlighted portfolio items with hover effect.

### Team Section

- **Card Hover Effect**: Applied hover effect to team member cards for consistency.

### Contact Section

- **Form Label Styling**: Improved form usability with bold labels.

### Footer

- **Padding and Text Alignment**: Enhanced spacing and alignment for a clean layout.

### Back to Top Button

- **Position and Styling**: Added fixed position and hover effect for user convenience.

## JavaScript Enhancements

### Smooth Scrolling for Navigation Links

Implemented smooth scrolling for navigation links:

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

### Back to Top Button Functionality

Added a back-to-top button:

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

## Technologies Used

- **Bootstrap 5**: Front-end framework for responsive design.
- **HTML5**: Structure and content of the web pages.
- **CSS3**: Styling and customization.
- **JavaScript**: Enhancing interactivity.

## Contributors

- [Telesphore Uwabera](https://github.com/Telesphore-Uwabera)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

To visit the HD-Company website, click [here](https://telesphore-uwabera.github.io/HD-Company/).
