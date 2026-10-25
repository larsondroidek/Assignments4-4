# Assignment 4.4 — Solution: Metadata & Page Setup

## The Metadata Code (put inside `<head>` of EVERY HTML file)
```html
    <!-- Character encoding -->
    <meta charset="UTF-8" />
    <!-- Mobile viewport -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- Page title and description (shown in tabs and search results) -->
    <title>Code Corner | Home — Learn Web Development</title>
    <meta name="description" content="Code Corner is a small website where a student shares what they learn about HTML and web development." />
    <meta name="author" content="Your Name" />
    <!-- Favicon -->
    <link rel="icon" type="image/png" href="images/favicon.png" />
    <!-- Stylesheet -->
    <link rel="stylesheet" href="style.css" />
```
Change only the `<title>` and `description` per page (each page needs its own). Adjust the `href` paths if the page is in a subfolder (e.g. `../images/favicon.png`).

## Project Structure
```
two-page-website/
├── index.html
├── about.html
├── style.css
└── images/
    └── favicon.png
```
This example updates the two-page website (Assignment 3.1). Apply the same `<head>` to your other old projects (personal page, portfolio, college-info, forms, marksheet, club site).

## Step-by-Step
1. **UTF-8:** `<meta charset="UTF-8" />` as the first tag in `<head>` — makes symbols such as `©`, `—`, `&rarr;` display correctly.
2. **Viewport:** `<meta name="viewport" content="width=device-width, initial-scale=1.0" />` — lets the page scale on phones.
3. **Title:** unique and meaningful for each page, e.g. `Home | Code Corner`, `About | Code Corner`.
4. **Description:** one sentence (about 120–160 characters) that summarizes the page; search engines may show it under the title.
5. **Favicon:** `<link rel="icon" type="image/png" href="images/favicon.png" />` — the small icon in the browser tab.
6. **Verify CSS links and paths:** `<link rel="stylesheet" href="style.css" />`; the file must exist at that path.

## Suggested Titles and Descriptions for Your Earlier Projects
| File | Title | Description |
|------|-------|-------------|
| Assignment 2.5 `index.html` | Your Name — Personal Introduction | Personal introduction page of Your Name: about, education, skills, hobbies and contact. |
| Assignment 3.2 `index.html` | Your Name — Portfolio Gallery | Portfolio page with an image gallery. |
| Assignment 3.3 `college-info.html` | College Information — Bachelor of Computer Science | Course introduction, subjects, admission process and faculty details. |
| Assignment 3.5 `index.html` / `blog.html` | Your Name — Portfolio / Blog — Your Name | Portfolio and blog of Your Name. |
| Assignment 4.1 `registration.html` | Student Registration Form | Register as a student by filling in your details. |
| Assignment 4.2 `job-application.html` | Job Application Form | Apply for a job by submitting your details and cover letter. |
| Assignment 4.3 `marksheet.html` | Student Marksheet | Annual examination marks of Class 10-A. |

## How to Verify
1. Open `index.html` with Live Server; the favicon appears in the **browser tab** next to the title (hard refresh with `Ctrl + F5` if you do not see it; browsers cache favicons).
2. Press `F12` → **Network** tab → refresh: `style.css` and `favicon.png` must show status **200** (a 404 means a wrong path).
3. Press `F12` → **Elements** tab: confirm the `<head>` shows all the meta tags.
4. Resize the window or open the DevTools device toolbar (`Ctrl + Shift + M`) to check the mobile viewport.

I checked the attached files with a script: both pages have UTF-8, viewport, description and favicon, and every linked file (`style.css`, `images/favicon.png`, the other page) exists.

## Submission
- ✅ Updated HTML files and the metadata code (above)
- 📸 Browser screenshot where the **tab** shows the favicon and the page title
