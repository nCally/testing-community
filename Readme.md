# PreLaunch

PreLaunch is a modern, responsive landing page designed to connect visionary app builders with real-world testers. The platform helps builders get valuable feedback before launching, and allows testers to earn stipends for testing unreleased apps.

## Features

- **Modern Aesthetics:** Built with a dark mode "glassmorphism" design, smooth gradient accents, and micro-animations.
- **Targeted Messaging:** Dedicated sections outlining the value proposition for both app builders and testers.
- **Waitlist Integration:** Includes an email collection form with mock Google Form integration and spam-prevention tips (suggesting email aliases like iCloud+ or DuckDuckGo).
- **Zero Build Setup:** Built using pure HTML and Tailwind CSS v3 via CDN. No `npm` installation or build steps required.

## Getting Started

1. Clone or download this repository.
2. Open `index.html` directly in any modern web browser to view the landing page.

## Connecting the Google Form

To successfully collect email addresses from the waitlist form, you must connect it to your own Google Form:

1. **Create the Form:** Create a Google Form with two fields:
   - A multiple-choice question for "Role" with options: `Tester`, `App Builder`.
   - A short-answer text field for "Email Address".
2. **Find the Action URL:** 
   - Preview your Google Form.
   - Right-click and select "Inspect Element" to find the `<form>` tag.
   - Copy the URL inside the `action="..."` attribute.
   - Open `index.html` and replace the placeholder `YOUR_GOOGLE_FORM_ACTION_URL` with your copied URL.
3. **Map the Input Fields:**
   - In the inspector, find the `name` attribute for both of your inputs (they will look like `entry.1234567`).
   - In `index.html`, replace `entry.ROLE_ID` and `entry.EMAIL_ID` with your specific entry numbers.

## Technology Stack

- **HTML5**
- **Tailwind CSS v3** (via CDN)
- **Google Fonts** (Inter, Outfit)