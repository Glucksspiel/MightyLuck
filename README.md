Name: MightyLuck

Project: Portfolio

Live Link: (https://github.com/Glucksspiel/MightyLuck)

Tech Used: HTML / CSS / JavaScript

Goal: A website that presents my personal portfolio and links to sample projects.

Features:
- Light and Dark theme toggle (persists the user’s preference across visits)
- Project images link to GitHub project pages when clicked

Screenshots: 

Challenges & Fixes: 

Page flickered wrong theme on load because JS ran too late.
Moved critical theme setting code to an inline script in the <head> to load the correct theme instantly.


Next Step Ideas: I would like to improve design and add some more features but for now i dont have anything in my mind

ADDED 28/11/2025
Dual-Theme Logic:

Light Theme variables are set by default.

Dark Theme variables override the light theme when the <html> element has the attribute data-theme="dark".

System Preference: A @media (prefers-color-scheme: dark) block is included to apply the dark theme variables automatically if the user's operating system is set to dark mode, unless a data-theme attribute is already set.

Aesthetics (Post-Enhancement):

Uses the Poppins font for a modern look.

Project cards have a clean border, background, and a subtle box shadow.

Hover Animation: Project cards lift slightly (transform: translateY(-5px)) and their shadow grows on hover for a dynamic effect.

Transitions: The transition: background var(--transition), color var(--transition) property is applied globally to ensure color changes (like switching themes) are smooth and animated, rather than instant.
