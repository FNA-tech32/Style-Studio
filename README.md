# Style Studio — Premier Hair Salon & Barber Web Application

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-4.x-purple.svg)](https://getbootstrap.com/)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)]()

Welcome to the official repository for **Style Studio**, a modern, responsive web application designed for a premier hair salon and barbershop. The platform allows clients to explore grooming and styling services, view transparent pricing, meet expert stylists and master barbers, browse an interactive portfolio lookbook, read and submit client reviews with an interactive star rating system, reserve appointments online, and connect directly with the studio through multiple primary and alternative contact channels.

---

## Table of Contents

- [About Style Studio](#about-style-studio)
- [Key Features](#key-features)
- [Services & Pricing](#services--pricing)
- [Contact Details & Alternative Channels](#contact-details--alternative-channels)
- [Behavior Driven Development (BDD)](#behavior-driven-development-bdd)
- [Technologies Used](#technologies-used)
- [File & Folder Structure](#file--folder-structure)
- [Installation & Local Setup](#installation--local-setup)
- [Development & Contribution](#development--contribution)
- [License](#license)

---

## About Style Studio

**Style Studio** operates as an elite salon and grooming lounge located at **The Junction Mall (Ground Floor, Room 32)** along Ngong Road, Nairobi, with an alternative studio location at **Westgate Shopping Mall, Westlands**. 

Staffed by over twenty-five certified beauty professionals—including 15 expert salonists and 10 master barbers—Style Studio offers parallel grooming stations capable of serving multiple clients simultaneously without sacrificing personal care or precision. The platform eliminates long waiting queues by enabling seamless digital appointment reservations.

---

## Key Features

1. **Responsive Hero Showcase**
   - Animated carousel banner introducing the **Style Studio** brand and ethos.
   - Quick navigation buttons to jump directly to appointment booking or services.

2. **Curated Services Showcase**
   - Clean display of signature treatments including Braiding, Trimming, Dreadlocks, Hair Coloring, and more.
   - Upfront pricing displayed for customer transparency.

3. **Stylist & Barber Team Profiles**
   - Highlighting experienced team members (Stylists, Master Barbers, Manicurists) along with their social media links.

4. **Customer Style Portfolio**
   - Interactive visual gallery displaying real client styles (Hair cuts, Cornrows, Blow outs, Beard & mustache trims, Hair coloring, Clean cuts, Dreadlocks, and Head & neck massages).
   - Lightbox image preview using Magnific Popup.

5. **Client Testimonials & Interactive 5-Star Rating**
   - Dynamic reviews slider powered by Owl Carousel.
   - Interactive star rating system allowing visitors to rate their experience with instant visual feedback.

6. **Online Appointment Booking System**
   - Dedicated reservation form to book visits by selecting preferred date, service type, and adding special requests or stylist preferences.
   - Available on both the main landing page and as a standalone booking module (`booking.html`).

7. **Direct Contact Hub & Alternative Communication Channels**
   - AJAX-powered contact form with real-time validation via `jqBootstrapValidation` and PHP mailer handler.
   - Dedicated contact cards highlighting both **Primary** and **Alternative** contact channels (Phone, WhatsApp, Email, Multiple Physical Locations, and Operating Hours).

---

## Services & Pricing

| Service | Category | Indicative Price |
| :--- | :--- | :--- |
| **Braiding** | Styling & Protective Care | Ksh. 500 |
| **Trimming** | Barbering & Hair Grooming | Ksh. 200 |
| **Dreadlocks** | Creation & Maintenance | Ksh. 2,500 |
| **Coloring** | Treatment & Tints | Ksh. 700 |
| **Shave & Clean Cut** | Precision Barbering | Custom / On Consultation |
| **Texturizing & Conditioning**| Treatment & Hair Care | Custom / On Consultation |
| **Nail Services** | Grooming & Manicure | Custom / On Consultation |

---

## Contact Details & Alternative Channels

Style Studio offers multiple communication channels to ensure quick support, effortless booking, and client accessibility:

| Channel | Primary Detail | Alternative Detail | Notes |
| :--- | :--- | :--- | :--- |
| **Phone** | `+1 (555) 234-5678` | `+1 (555) 987-6543` | Direct line & phone support |
| **WhatsApp / Instant Messaging** | `+1 (555) 987-6543` | `+254 798 765 432` | Instant booking & consultations |
| **Email** | `info@stylestudio.com` | `appointments@stylestudio.com` | Inquiries & appointment requests |
| **Support Email** | `support@stylestudio.com` | `feedback@stylestudio.com` | Customer feedback & support |
| **Main Studio Location** | Room 32, Ground Floor, The Junction Mall, Ngong Road, Nairobi, Kenya | — | Full salon & barbershop services |
| **Alternative Branch** | 2nd Floor, Westgate Shopping Mall, Westlands, Nairobi, Kenya | — | Alternative branch location |
| **Working Hours** | **Mon – Fri:** 8:00 AM – 8:00 PM | **Sat – Sun:** 9:00 AM – 6:00 PM | Public Holidays: 10:00 AM – 4:00 PM |

---

## Behavior Driven Development (BDD)

### 1. Appointment Booking Form

| Action / Behavior | User Input | Expected System Output |
| :--- | :--- | :--- |
| **Enter Personal Details** | First Name, Last Name, Email | Inputs validated for correct formatting. |
| **Select Date** | Desired reservation date | Calendar date selected for appointment scheduling. |
| **Select Service** | Haircut, Coloring, Dreadlocks, etc. | Service type recorded for booking reservation. |
| **Add Special Notes** | Custom requests, hair specifications | Notes appended to the booking ticket. |
| **Submit Form** | Clicks **"Confirm Booking"** | Form submitted and reservation recorded. |

### 2. Interactive Rating System

| Action / Behavior | User Input | Expected System Output |
| :--- | :--- | :--- |
| **Hover on Star** | Moves cursor over 1st to 5th star | Stars up to hovered star highlight in golden color. |
| **Click Star Rating** | Clicks on 4th or 5th star | Selected rating locked; thank you message with success checkmark displayed. |

### 3. Contact Form Submission

| Action / Behavior | User Input | Expected System Output |
| :--- | :--- | :--- |
| **Incomplete Form** | Empty required field | Form displays validation warning and highlights field. |
| **Valid Submission** | Name, Valid Email, Phone, Message | AJAX triggers `mail/contact_me.php`, displays success alert, and clears inputs. |

---

## Technologies Used

- **Markup & Styling:** HTML5, CSS3, SCSS
- **Front-end Framework:** [Bootstrap 4](https://getbootstrap.com/)
- **Scripting & Interactivity:** JavaScript (ES6+), [jQuery](https://jquery.com/)
- **Icons & Typography:** [FontAwesome 4.7](https://fontawesome.com/v4/), Google Fonts (*Lobster*, *Roboto*, *Great Vibes*, *Bree Serif*)
- **Animation & Transitions:** [WOW.js](https://wowjs.uk/), [Animate.css](https://animate.style/)
- **Interactive Plugins:** [Owl Carousel 2](https://owlcarousel2.github.io/OwlCarousel2/), [Swiper.js](https://swiperjs.com/), [Magnific Popup](https://dimsemenov.com/plugins/magnific-popup/)
- **Form Validation:** `jqBootstrapValidation`
- **Backend Communication:** PHP mail handler (`mail/contact_me.php`)

---

## File & Folder Structure

```
Style-Studio/
├── index.html                   # Main landing page for Style Studio
├── booking.html                 # Standalone online appointment reservation page
├── README.md                    # Project documentation and specifications
├── LICENSE                      # MIT Open Source License
├── css/                         # Compiled stylesheets & vendor CSS
│   ├── app.css                  # Core application stylesheet
│   ├── bootstrap.css            # Bootstrap core CSS
│   ├── animate.min.css          # Animation library
│   ├── magnific-popup.css       # Lightbox modal stylesheet
│   ├── owl.carousel.min.css     # Owl Carousel slider style
│   ├── owl.theme.default.min.css# Owl Carousel default theme
│   └── swiper.min.css           # Swiper carousel style
├── js/                          # Application scripts & vendor libraries
│   ├── app.js                   # Main application JavaScript (scroll, sliders, rating)
│   ├── contact_me.js            # AJAX contact form submission handler
│   ├── contact_me.min.js        # Minified contact form script
│   ├── jqBootstrapValidation.min.js # Form validation script
│   ├── jquery.min.js            # jQuery core library
│   ├── bootstrap.min.js         # Bootstrap JavaScript bundle
│   ├── owl.carousel.min.js      # Slider plugin
│   ├── swiper.min.js            # Swiper plugin
│   └── wow.min.js               # Scroll reveal animation plugin
├── img/                         # Website imagery
│   ├── client/                  # Client review avatars & photos
│   ├── portfolio/               # Customer hair & styling gallery images
│   ├── service/                 # Service showcase imagery
│   ├── team/                    # Stylist & barber team portrait photos
│   └── logo.png                 # Studio brand logo
├── mail/                        # Backend mail processor
│   └── contact_me.php           # PHP script handling contact messages
└── scss/                        # Source SASS/SCSS files
    ├── app.scss                 # Master SCSS file compiling all modules
    ├── _navbar.scss             # Navbar styling
    ├── _masthead.scss           # Hero header & carousel styling
    ├── _services.scss           # Service cards styling
    ├── _about.scss              # About us section styling
    ├── _team.scss               # Team cards styling
    ├── _portfolio.scss          # Portfolio lookbook styling
    ├── _testimonials.scss      # Testimonial slider & rating styling
    ├── _contact.scss            # Contact section styling
    └── _footer.scss             # Footer styling
```

---

## Installation & Local Setup

To run or develop the project locally on your machine:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/YourUsername/Style-Studio.git
   cd Style-Studio
   ```

2. **Open the project:**
   - **Direct Browser Execution:** Double-click `index.html` or open it with any web browser (Chrome, Firefox, Edge, Safari).
   - **Live Server (Recommended):** If using VS Code, right-click `index.html` and select **"Open with Live Server"**, or run a lightweight local server:
     ```bash
     # Using Python 3
     python -m http.server 8000
     ```
     Then navigate to `http://localhost:8000` in your web browser.

3. **Standalone Booking Page:**
   - Open `booking.html` directly in your browser to view the isolated reservation workflow.

---

## Development & Contribution

We welcome contributions to enhance Style Studio! To contribute:

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/NewFeature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new styling feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/NewFeature
   ```
5. Open a Pull Request detailing your changes.

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for complete details.

&copy; 2026 **Style Studio**. All Rights Reserved.
