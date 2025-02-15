# Accessible Nature Site

This project is a fictional nature site displaying an article about bears. The site had several **accessibility issues**, which have now been **fixed** to ensure it is **usable for all users**, including those with **visual impairments, keyboard navigation needs, and screen readers**.

## Getting Started

To get started, clone this repository and open the `index.html` file in your browser.  

Alternatively, use **VSCode Live Server** for real-time updates. No additional setup is required.

## Accessibility Improvements

### Color Contrast Fix
- **Issue:** The original text/background contrast was too low, making it hard to read.
- **Fix:** Updated colors to meet **WCAG AA contrast standards** for readability.

### Semantic HTML & Navigation
- **Issue:** The `<div class="nav">` structure was not properly accessible.
- **Fix:** Changed it to a **`<nav>` element** to improve keyboard and screen reader navigation.

### Improved Headings & Content Structure
- **Issue:** `<font>` tags were used instead of proper headings (`<h1>`, `<h2>`, etc.).
- **Fix:** Replaced `<font>` with **semantic headings**, making navigation easier.

### image Accessibility
- **Issue:** Images lacked **alt text**, making them invisible to screen readers.
- **Fix:** Added **descriptive `alt` attributes** for each image.

### Accessible Audio Player
- **Issue 1:** No transcript for hearing-impaired users.
- **Fix:** Added a **text transcript** below the audio player.
- **Issue 2:** No fallback for older browsers.
- **Fix:** Provided a **download link** in case the `<audio>` element isn't supported.

### Search Form Label (Hidden for Sighted Users)
- **Issue:** The search bar had no label, making it difficult for screen readers.
- **Fix:** Added an **invisible `<label>`** using `aria-label`.

### Comment Form Fixes
- **Issue:** Labels were not correctly linked to input fields.
- **Fix:** Used **`<label for="inputID">`** to explicitly associate labels.

### Keyboard-Accessible Show/Hide Button
- **Issue:** The **show/hide comments** button was not focusable via keyboard.
- **Fix:** Added `tabindex="0"` and `keydown` event listener to allow **keyboard interaction**.

### Improved Table Accessibility
- **Issue 1:** No summary or clear headers.
- **Fix:** Added:
  - `<caption>` for a **visible title**
  - `<p id="table-summary" hidden>` for **screen readers**
- **Issue 2:** Difficult to distinguish rows/columns.
- **Fix:** Applied **color differentiation** for headers and first column.

## Development

To make additional changes, simply edit the **HTML, CSS, and JavaScript** files in this project.

## Testing

To ensure all accessibility features work:
1. Navigate using the **keyboard (Tab key)**
2. Use a **screen reader** (e.g., VoiceOver, NVDA)
3. Check **color contrast** using online tools

---

This project follows **Web Content Accessibility Guidelines (WCAG 2.1)** to improve usability for all users.
