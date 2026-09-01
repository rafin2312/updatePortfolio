MD. Kamran Hasan Rafin — Software Engineer Portfolio

<p align="center">
<a href="https://rafin2312.github.io/updatePortfolio/">
    <img src="https://img.shields.io/badge/Live%20Portfolio-Visit%20Site-8B6DFF?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Visit live portfolio">
  </a>
  <a href="https://github.com/rafin2312/updatePortfolio">
    <img src="https://img.shields.io/badge/Source%20Code-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="View source code on GitHub">
  </a>
</p> <p align="center">
  <strong>A responsive, interactive personal portfolio for software engineering, machine learning research, computer networking, and creative work.</strong>
</p> <p align="center">
  <a href="https://rafin2312.github.io/updatePortfolio/">Live Demo</a> ·
  <a href="https://github.com/rafin2312">GitHub Profile</a> ·
  <a href="mailto:mdkamranhasanrafin@gmail.com">Contact</a>
</p>




Overview

This repository contains the source code for the personal portfolio of Md. Kamran Hasan Rafin, a Computer Science and Engineering undergraduate at Southeast University, Dhaka. The portfolio presents a technical profile through a polished, glassmorphism-inspired interface built with web standards and lightweight client-side JavaScript.

The site is designed to communicate both technical depth and personality. It brings together software engineering projects, applied machine learning research, computer networking interests, professional experience, education, photography, and contact information in a single responsive experience.


Design direction: The visual system uses a dark “Signal Spectrum” theme inspired by network topologies, explainable-AI heatmaps, activation gradients, and data visualisation interfaces.

Live Portfolio

Visit the deployed portfolio at rafin2312.github.io/updatePortfolio.

Highlights

Area
What the portfolio presents
Software Engineering
Java, C++, object-oriented programming, algorithms, data structures, and practical application design.
Artificial Intelligence & ML
Applied machine learning, predictive modelling, deep learning, and explainable AI.
Computer Networking
Cisco networking, protocol behaviour, infrastructure design, packet analysis, latency, and traffic flow.
Research
PlantVisionBD, a plant disease detection study using EfficientNetV2L with Grad-CAM and SHAP analysis.
Professional Profile
IT operations experience, technical support, stakeholder communication, and infrastructure reliability.
Creative Work
Travel and landscape photography from trekking experiences in Bangladesh.




Core Features

Interactive Portfolio Experience

The hero section includes a dynamic typing effect that cycles through role descriptors such as AI Enthusiast, ML Researcher, Problem Solver, and CS Student. Animated counters communicate selected portfolio metrics, while a persistent spectrum bar, layered glow effects, and grid styling establish the site's visual identity.

Responsive Glassmorphism Interface

The layout uses translucent cards, blur effects, gradient borders, custom CSS variables, responsive grids, and mobile navigation. The interface is designed to remain usable across desktop, tablet, and mobile screen sizes, including a hamburger menu and mobile overlay.

Scroll-Aware Interactions

Sections and content cards use IntersectionObserver-based reveal animations. The navigation bar changes state after scrolling, and the active navigation item updates according to the section currently in view. Skill bars animate when they enter the viewport.

Research Showcase

The featured research section documents PlantVisionBD: Plant Disease Detection Using EfficientNetV2L with Explainable AI. It presents the study's reported performance metrics, technical approach, research highlights, and a link to the full paper included in the repository.

Project Showcase

The technical projects section includes:

Project
Description
Technologies
Enterprise Java System
An object-oriented software application focused on scalable data structures and runtime performance.
Java, OOP
Advanced Algorithmic Suite
Algorithmic problem-solving work involving dynamic programming, resource allocation, complexity, and memory analysis.
C++, Data Structures
Network Infrastructure Project
An in-progress hands-on project involving topology design, protocols, traffic behaviour, packet loss, and latency analysis.
Networking, Cisco, Protocols
Student Management System
A command-line Java application for managing student records.
Java, OOP, Console
Exam Management System
A JavaFX desktop application for managing exams through an event-driven graphical interface.
Java, JavaFX, GUI




Photography Gallery and Lightbox

The “Beyond the Code” section includes a featured photography area with paginated image rendering and a lightbox viewer. Images follow a predictable naming convention such as photo1.jpg, photo2.jpg, and so on, making the gallery straightforward to maintain.

Technology Stack

Layer
Technologies
Markup
HTML5, semantic sections, accessible labels, and responsive viewport metadata
Styling
CSS3, custom properties, Flexbox, CSS Grid, gradients, transitions, animations, and glassmorphism effects
Interactivity
Vanilla JavaScript, DOM APIs, IntersectionObserver, scroll state handling, animated counters, typing effects, navigation controls, pagination, and lightbox logic
Typography
Space Grotesk, Inter, and JetBrains Mono via Google Fonts
Icons
Font Awesome 6
Hosting
GitHub Pages-compatible static deployment




Repository Structure

Plain Text


updatePortfolio/
├── .github/
│   └── workflows/                  # Repository workflow configuration
├── index.html                      # Main portfolio markup and client-side scripts
├── style.css                       # External stylesheet and supporting styles
├── profile.JPG                     # Profile image used in the hero section
├── photo1.jpg ... photo8.jpg       # Photography gallery assets
├── plantvisionbd-paper.pdf         # Featured research paper
├── MD_Kamran_Hasan_Rafin_CV.pdf    # Downloadable curriculum vitae
└── README.md                       # Project documentation



Run Locally

Because this is a static front-end project, no build system or package installation is required.

1. Clone the repository

Bash


git clone https://github.com/rafin2312/updatePortfolio.git
cd updatePortfolio



2. Start a local server

You can open index.html directly in a browser, but a local HTTP server is recommended so that assets and browser APIs behave consistently.

Bash


python3 -m http.server 8000



Then open http://localhost:8000 in your browser.

3. Stop the server

Press Ctrl+C in the terminal running the server.

Customization Guide

Update Personal Information

Edit the hero, About Me, experience, education, and contact sections in index.html. The primary email address, location, social profiles, résumé link, and research-paper link are all defined in the markup and can be updated without changing the JavaScript.

Add or Replace Projects

Duplicate one of the existing project cards in the Technical Projects section, update its title, description, technology labels, and GitHub URL, then remove or reorder cards as needed.

Maintain the Photography Gallery

Place images in the project root using sequential filenames:

Plain Text


photo1.jpg
photo2.jpg
photo3.jpg
...



Update TOTAL_PHOTOS in the JavaScript near the bottom of index.html whenever images are added or removed. The gallery automatically separates the first three images into the Featured area and paginates the remaining images.

JavaScript


const TOTAL_PHOTOS = 8;
const PHOTOS_PER_PAGE = 9;



Adjust the Visual Theme

The primary colours, typography, backgrounds, borders, and gradients are defined through CSS custom properties near the beginning of index.html. The most important variables include:

CSS


:root {
  --bg-main: #07060D;
  --violet: #8B6DFF;
  --cyan: #2BE4FF;
  --emerald: #16EFA8;
  --rose: #FF5C82;
}



Changing these variables is the quickest way to create a new colour direction while preserving the existing component system.

Deployment

The project is structured as a static website and can be deployed through GitHub Pages or any static hosting provider.

For GitHub Pages:

1.
Push the repository to GitHub.

2.
Open the repository's Settings page.

3.
Select Pages under the repository configuration.

4.
Choose the deployment source and the main branch.

5.
Save the configuration and wait for GitHub Pages to publish the site.

After deployment, verify that relative assets such as profile.JPG, gallery images, the CV, and plantvisionbd-paper.pdf are loading correctly.

Accessibility and Performance Notes

The portfolio uses semantic section identifiers, descriptive navigation labels, responsive layout rules, and accessible labels for icon-only social controls. For future improvements, image alt text should be reviewed whenever new gallery or profile assets are added, and large images should be compressed before deployment to keep page loading fast.

The site intentionally avoids a framework and build dependency, which keeps the deployment surface small and makes the portfolio easy to inspect, fork, and host. External font and icon resources are loaded from their respective CDNs, so an internet connection is required for those resources to render as intended.

Roadmap

Status
Planned improvement
In progress
Complete and publish the network infrastructure project with a dedicated repository link.
Planned
Add dedicated project pages with screenshots, architecture notes, and implementation details.
Planned
Add a downloadable project résumé or case-study format for selected work.
Planned
Improve image optimisation and add more detailed alternative text for gallery content.
Planned
Add automated HTML, accessibility, and link checks to the repository workflow.




Contact

I am open to software engineering opportunities, internships, machine learning research collaborations, networking projects, and thoughtful technical conversations.

Channel
Link
Email
mdkamranhasanrafin@gmail.com
GitHub
github.com/rafin2312
LinkedIn
linkedin.com/in/rafin2312
Instagram
@hardin_2312
Location
Dhaka, Bangladesh




License

No license file is currently included in the repository. If you want others to reuse, modify, or redistribute the portfolio source code, add an appropriate open-source license such as the MIT License and update this section accordingly. Until then, treat the source code, written content, résumé, research paper, and personal media as the author's original work and request permission before reuse.

References

[1] updatePortfolio source repository
[2] Rafin's live portfolio
[3] Rafin's GitHub profile
[4] PlantVisionBD research paper
[5] Md. Kamran Hasan Rafin CV



<p align="center">
Designed and developed by <strong>Md. Kamran Hasan Rafin</strong> · © 2026
</p>
