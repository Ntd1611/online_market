# Project Requirements Document: Bảo Trâm Mart Website Frontend

**Version:** 1.0
**Date:** 2023-10-27

## 1. Introduction

### 1.1. Project Overview
This document outlines the requirements for the **frontend** development of the official website for Bảo Trâm Mart, a grocery store located in Đà Nẵng, Vietnam. The website will serve as an online presence to inform customers about weekly specials, store information, and potentially other relevant content like recipes.

### 1.2. Project Goal
The primary goal is to create a modern, user-friendly, and informative website that reflects the Bảo Trâm Mart brand, attracts customers, and provides easy access to key information, primarily weekly specials and store details. It should enhance the store's visibility and provide a convenient way for customers to check promotions before visiting.

### 1.3. Inspiration & Design Direction
*   **Functional Structure:** The website structure and core features (Flyer/Specials, Store Info, Contact) should be similar to `https://www.supermarchepa.com/`.
*   **UI/UX:** The user interface should be **modernized** compared to the reference site. It should incorporate the Bảo Trâm Mart branding (logo, colors from provided images), use high-quality imagery, and prioritize a clean, intuitive, and visually appealing experience, especially on mobile devices.
*   **Branding Assets:** Utilize the provided logo, color palette (greens, yellows, creams), and potentially font styles suggested by the banner image. Incorporate the tagline "SMART CHOICE MAKE BETTER LIFE".

## 2. Target Audience

*   Current and potential customers of Bảo Trâm Mart in the Đà Nẵng area.
*   Individuals looking for grocery specials, specific products (potentially imported goods based on images), or gift baskets in the region.
*   Users accessing the site via both desktop and mobile devices.

## 3. Scope

### 3.1. In Scope (Frontend Only)
*   Development of all user-facing website components using HTML, CSS, and JavaScript (and a chosen framework/library).
*   Implementation of the visual design and user interface based on approved mockups/style guides (to be created).
*   Integration with **placeholder/mock data** or a **pre-defined API structure** for dynamic content like flyer items, store hours, and recipes. *Actual backend/API development is out of scope.*
*   Responsive design ensuring optimal viewing and interaction across various screen sizes (desktop, tablet, mobile).
*   Implementation of features detailed in the Functional Requirements section.
*   Basic SEO meta tags implementation (titles, descriptions).
*   Primary language: **Vietnamese**.

### 3.2. Out of Scope
*   Backend development (server logic, database, API creation).
*   Content Management System (CMS) integration (unless specified as a requirement for fetching data via API).
*   User accounts, login/registration functionality.
*   E-commerce functionality (online ordering, shopping cart, checkout).
*   Content creation (text, final product images, recipe details - placeholder content will be used).
*   Hosting setup and deployment (beyond providing the build files).
*   Advanced SEO optimization or marketing campaigns.
*   English language version (unless added as a specific requirement later).

## 4. Functional Requirements

### 4.1. Global Elements
*   **Header:**
    *   Bảo Trâm Mart Logo (linking to Homepage).
    *   Main Navigation Menu (e.g., Khuyến Mãi [Specials/Flyer], Cửa Hàng [Store Info], Công Thức [Recipes], Liên Hệ [Contact]).
    *   (Optional) Search Bar - Primarily for searching within specials/products shown.
    *   Responsive: Collapses into a hamburger menu on smaller screens.
*   **Footer:**
    *   Copyright information (`© [Year] Bảo Trâm Mart`).
    *   Basic contact info (Address, Hotline).
    *   Links to key pages (e.g., Privacy Policy, Terms - if applicable).
    *   (Optional) Social media links.

### 4.2. Pages / Sections

*   **Homepage (`/`)**
    *   **Hero Section:** Visually engaging banner, potentially featuring current key promotions or branding (incorporating tagline).
    *   **Current Specials Highlight:** A section prominently displaying the current weekly flyer or key promotional items. Could be a link/button to the full flyer page or show a few top deals directly.
    *   **Featured Recipes (Optional):** A small section linking to recent or popular recipes.
    *   **Store Info Snippet:** Quick view of address and hours, with a link to the full Store Info page/section.
    *   **Call-to-Actions:** Clear prompts, e.g., "Xem Khuyến Mãi Tuần Này" (View This Week's Specials), "Tìm Cửa Hàng" (Find Store).

*   **Specials / Flyer Page (`/khuyen-mai` or `/flyer`)**
    *   **Primary Feature:** Display the current weekly specials.
    *   **Modern Implementation:** Instead of just a PDF viewer (like PA sometimes uses), consider a more integrated approach:
        *   **Option A (Interactive Viewer):** An embedded interactive flyer viewer (if a suitable tool/service is used).
        *   **Option B (Product Grid):** Display specials as a grid of products (image, name, price). This often feels more modern and web-native. Allows for filtering/searching within specials.
    *   Clear indication of the validity dates for the specials.
    *   Easy navigation between pages/sections of the flyer/specials list.
    *   Ability to view previous flyers (optional).

*   **Store Information Page / Section (`/cua-hang` or `/lien-he`)**
    *   **Contact Details:** Full Address (44 Phan Đình Phùng, Hải Châu, Đà Nẵng), Hotline (0236 6288 099, potentially others from image watermark).
    *   **Opening Hours:** Clearly listed hours for each day of the week.
    *   **Map:** Embedded interactive map (e.g., Google Maps) showing the store location.
    *   (Optional) Contact Form.

*   **Recipes Page (`/cong-thuc`) (Optional but Recommended)**
    *   **Recipe Listing:** Grid or list view of available recipes. Each entry shows image, title, brief description.
    *   **Recipe Detail View:** When a recipe is clicked, show ingredients, instructions, prep/cook time, servings, larger image/video.
    *   (Optional) Categorization or search for recipes.

*   **Search Functionality (If Implemented)**
    *   Input field (likely in the header).
    *   Displays results, primarily focusing on products found within the current specials/flyer.

## 5. Non-Functional Requirements

*   **Performance:** Fast loading times (optimized images, efficient code). Aim for good Core Web Vitals scores.
*   **Responsiveness:** Fully responsive design adapting seamlessly to desktop, tablet, and mobile viewports (mobile-first approach recommended).
*   **Cross-Browser Compatibility:** Works correctly on latest versions of major browsers (Chrome, Firefox, Safari, Edge).
*   **Usability:** Intuitive navigation, clear layout, easy to find key information (specials, store location/hours).
*   **Accessibility:** Adherence to basic WCAG (Web Content Accessibility Guidelines) principles (e.g., semantic HTML, alt text for images, sufficient color contrast).
*   **Maintainability:** Clean, well-commented, and organized code structure. Use of a modern frontend framework/library (e.g., React, Vue, Angular, Svelte) is recommended.
*   **Security:** Frontend security best practices (e.g., preventing XSS if user input is ever displayed, though minimal in this scope).

## 6. Design & UI/UX Requirements

*   **Modern Aesthetic:** Clean lines, ample whitespace, intuitive layout. Avoid cluttered interfaces.
*   **Branding:** Consistently use the Bảo Trâm Mart logo, color scheme (greens, yellows, creams from provided images), and typography that aligns with the brand. Incorporate the tagline "SMART CHOICE MAKE BETTER LIFE" where appropriate (e.g., homepage, footer).
*   **Imagery:** Use high-quality, appealing images of food, products, and potentially the store environment. Ensure images are optimized for web use.
*   **Typography:** Choose readable, modern fonts (likely sans-serif) suitable for both Vietnamese and potentially English text if added later. Ensure appropriate font sizes and line heights for readability.
*   **Interactivity:** Use subtle animations or transitions to enhance user experience where appropriate, without sacrificing performance. Ensure interactive elements (buttons, links) have clear hover and active states.
*   **Wireframes/Mockups:** Detailed wireframes and high-fidelity mockups should be created and approved before development begins, defining the layout, components, and user flow for all pages and screen sizes. [Link to Figma/Design Mockups - Placeholder]

## 7. Technology Stack (Recommendation)

*   **HTML5:** Semantic markup.
*   **CSS3:** Styling. Consider using a utility-first framework like **Tailwind CSS** for modern styling and responsiveness, or a component library like **Bootstrap 5**.
*   **JavaScript (ES6+):** For interactivity.
*   **Frontend Framework/Library:** **React**, **Vue.js**, or **Angular** recommended for building modular and maintainable components. A static site generator (like Next.js, Nuxt.js, Astro) could also be suitable for performance if backend interaction is minimal.
*   **Version Control:** Git (e.g., using GitHub, GitLab, Bitbucket).

## 8. Future Considerations (Post Initial Launch)

*   Full E-commerce functionality (product catalog, cart, checkout).
*   User accounts.
*   Integration with a CMS for easier content updates (flyers, recipes).
*   Blog section.
*   English language version.
*   More advanced search functionality (e.g., searching all site content).

## 9. Open Questions / Assumptions

*   Assumption: An API endpoint structure will be defined for fetching dynamic data (flyer items, recipes, store hours).
*   Assumption: All necessary branding assets (high-res logo, specific color codes) and content (text, final images) will be provided.
*   Question: Is the "Recipes" section a definite requirement for V1?
*   Question: What is the preferred method for displaying the flyer/specials (interactive viewer vs. product grid)?