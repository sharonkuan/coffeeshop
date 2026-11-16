# The Corner Cafe ☕🍰🐾

## Project Overview

The Corner Cafe is a responsive Bootstrap website created as part of the Nucamp Web Fundamentals Workshop. The project began as an adaptation of the Nucampsite coursework project and was transformed into a fictional neighborhood coffee shop website.

Development began using an enhanced version of the Nucampsite project that incorporated prior optional coursework exercises, including Bootstrap card-based layouts. Reusing this work provided a stronger foundation for the coffee shop redesign and allowed more development time to be spent on branding, user experience improvements, ordering functionality, and deployment.

The primary objective of this workshop was to apply the concepts learned throughout the Web Fundamentals cohort, including responsive design, Bootstrap components, SCSS, and Firebase deployment. Beyond the required coursework, I customized the application to fit a coffee shop business concept, explored AI-assisted development workflows, and implemented additional functionality to enhance the user experience.

The project demonstrates my ability to adapt and extend existing templates by modifying layouts, content, styling, and functionality while ensuring that component relationships, IDs, and Bootstrap behaviors continue to function correctly.

The project was completed in approximately 9 hours, including design, implementation, debugging, testing, and Firebase deployment.

## Live Site

Firebase Hosted Site:

https://sharonk-thecornercafe-2026.web.app/index.html

---

## Project Goals

This project was designed to demonstrate:

- Responsive web design
- Bootstrap components and layouts
- SCSS styling and organization
- JavaScript-enhanced user interactions
- Firebase deployment
- AI-assisted design and development

Instead of recreating every page from scratch, I intentionally reused portions of the original Nucampsite project and focused development time on customization, branding, functionality, usability, and deployment.

---

## Design Journey

The project initially started with the Nucampsite Home page.

As development progressed, I reimagined the site as a neighborhood coffee shop centered around:

- Coffee
- Cakes and pastries
- Take-out ordering
- Pet-friendly experiences
- Community gathering

During development, I used Microsoft Copilot to help generate branding concepts, logos, promotional images, website content, banner text, and image captions.

The design evolved iteratively as the branding and imagery were refined.

---

## Site Structure

The site consists of two primary pages:

### Home Page

- Hero section and branding
- Image carousel
- Promotional cards
- Coffee ordering modal

### About Page

- Business information
- Contact information
- Customer feedback form

To reduce development time, I repurposed the original Nucampsite Contact page into an About page while retaining the feedback form functionality.

This allowed me to spend more time building custom features and improving the user experience.

---

## Key Features

### Responsive Image Carousel

The homepage includes a Bootstrap carousel featuring custom imagery created specifically for The Corner Cafe.

Features include:

- Automatic slide rotation
- Indicators
- Previous and Next controls
- Responsive captions

---

### Custom Branding

The project includes:

- Custom Sharon logo
- AI-generated promotional images
- Consistent color themes
- Marketing content and captions

One design decision involved displaying the logo in both the header and navigation bar.

Initially, this was questioned because the branding appeared twice. However, I intentionally retained the logo in the sticky navigation bar because users continue seeing the navigation while scrolling. This helps maintain brand visibility and reinforces the identity of the coffee shop.

---

### Homepage Flow Improvement

While reviewing the homepage layout, I noticed that the carousel and feature cards appeared visually crowded.

To improve the visual flow, I added a banner section:

> ☕ Love is Best Shared Over Coffee & Cake ❤️

This created a natural transition between the carousel and promotional cards while reinforcing the site's theme.

---

### Sticky Navigation Ordering Button

A prominent Pre-order! button was added directly to the Bootstrap navigation bar.

Benefits include:

- Always visible while browsing
- Available from every page
- Improved customer access to ordering

Button placement required additional testing because its position affected visibility on smaller screen sizes.

---

## Multi-Item Coffee Ordering System

The project includes a custom Bootstrap ordering modal.

Customers can:

- Select coffee size
- Select quantity
- Add multiple coffees to an order
- Remove individual items
- Submit multiple coffee selections as a single order

Orders containing duplicate sizes automatically combine quantities for improved usability.

This functionality extends beyond the original workshop requirements.

---

## Cross-Page Modal Navigation

One of the most interesting implementation challenges involved allowing customers to begin an order from the About page.

### Original Goal

About Page

↓

Click Pre-order

↓

Home Page Modal Opens

### Initial Attempt

The first implementation used a button approach that did not successfully open the modal after navigating to another page.

### Final Solution

About Page

↓

Anchor Link

(index.html#reserve)

↓

Home Page Loads

↓

JavaScript Detects URL Hash

↓

Bootstrap Modal Opens Automatically

This required modifications to navigation and JavaScript logic and provided experience working with cross-page interactions.

---

## SCSS and Styling Organization

The project uses SCSS to improve code organization and maintainability.

Enhancements included:

- Shared color variables
- Reusable styling definitions
- Consistent branding colors
- Simplified styling maintenance

During development I used Sass watch mode to automatically compile SCSS into CSS while making updates.

Later in development, the styling was refactored to use centralized theme variables so color changes could be managed consistently across multiple pages.

Although the project was structured using SCSS, the HTML pages reference the compiled CSS files rather than the SCSS source files. This approach allowed the site to be developed and tested using either:

npm start

or

Live Server

while still benefiting from SCSS organization and maintainability. The SCSS files served as the source of truth, while the compiled CSS files provided compatibility with browser-based development and deployment workflows.

---

## AI-Assisted Development

This project incorporated AI-assisted development throughout both the design and implementation process.

### Microsoft Copilot

Used for:

- Coffee shop concept development
- Sharon logo generation
- Promotional image creation
- Marketing content
- Image captions
- Banner messaging

### Claude AI

Used as a development assistant for:

- JavaScript implementation
- Bug troubleshooting
- Modal workflow improvements
- Cross-page navigation issues
- SCSS organization
- Styling cleanup and refactoring

At the time of this project, I had previous experience working with JavaScript and C# in QA automation environments, but I had not yet formally studied JavaScript application development.

Rather than writing all JavaScript functionality from scratch, I focused on defining the desired user experience, testing functionality through the UI, identifying defects, describing unexpected behavior, and validating proposed solutions.

Examples included:

- Cross-page modal navigation
- Multi-item coffee ordering
- Error message handling
- Form interaction issues
- UI behavior corrections

AI-assisted solutions were tested and refined through multiple iterations until the functionality met the intended user experience.

This workflow closely reflected my QA background:

Define expected behavior

↓

Test implementation

↓

Identify issues

↓

Describe defects

↓

Apply fixes

↓

Retest

---

## Firebase Deployment

The Corner Cafe was deployed using Firebase Hosting.

During deployment, Firebase initialization initially failed even after creating a Firebase project and accepting the Terms of Service.

Investigation revealed that Firebase project IDs do not allow underscores (_).

After replacing underscores with dashes (-), deployment completed successfully.

This provided practical experience troubleshooting cloud deployment issues and hosting configuration.

---

## Technologies Used

### Front-End

- HTML5
- CSS3
- SCSS / Sass
- Bootstrap 5
- Font Awesome
- JavaScript

### Development Tools

- npm
- Parcel
- Git
- GitHub

### Hosting

- Firebase Hosting

### AI Tools

- Microsoft Copilot
- Claude AI

---

## Known Limitations

### Feedback Form

The feedback form currently:

- Accepts empty submissions
- Does not include client-side validation
- Would benefit from additional input validation

### Ordering System

Future enhancements may include:

- Coffee type selection
- Flavor options
- Milk options
- Additional beverages
- Bakery and dessert ordering
- Pricing calculations
- Order summaries
- Receipt generation

---

## Lessons Learned

This project provided practical experience in:

- Adapting an existing application to a new business concept
- Bootstrap component customization
- SCSS organization
- Responsive design
- Working with AI-assisted development tools
- Troubleshooting JavaScript-driven features
- Firebase deployment
- Iterative development practices

Most importantly, the project reinforced the value of:

Build

↓

Test

↓

Debug

↓

Improve

↓

Deploy

---

## Final Reflection

The Corner Cafe demonstrates how an existing project can be transformed into a completely different business application through customization, branding, AI-assisted development, and user-focused design decisions.

More than a workshop exercise, it became an opportunity to explore how modern developers combine frameworks, cloud services, AI tools, experimentation, testing, and problem solving to bring an idea from concept to deployment.

☕❤️🐾

*"Love is Best Shared Over Coffee & Cake."*