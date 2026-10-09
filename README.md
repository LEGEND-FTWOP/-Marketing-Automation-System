# MarketFlow

A clean, responsive Marketing Automation dashboard and landing page builder built with vanilla HTML, CSS, and JavaScript.

No frameworks, no build tools, no dependencies to install.

---

## Features

- **Authentication**: Sign in, register, and simulated Google SSO with session persistence.
- **Dashboard**: Track total campaigns, active campaigns, subscriber count, and email metrics.
- **Analytics**: Visual charts showing performance trends and open/click rates.
- **Campaigns**: View, search, and create new campaigns with A/B testing option.
- **Subscribers**: Manage subscribers and audience segments (VIP, Engaged, Inactive).
- **Templates**: Browse email templates with live responsive preview.
- **Workflow Builder**: Visual trigger-and-action automation pipeline.
- **Landing Page Builder**: Fullscreen drag-and-drop editor with inline text editing.
- **Dark Mode**: Quick toggle between light and dark themes.

---

## Quick Start

You don't need Node.js, npm, or any build setup.

1. Double-click **`index.html`** in your browser.
2. Sign in with any email and password (or click **"Sign in with Google"**).
3. You'll be taken straight to the dashboard.

*Optional: If you prefer running with a local server:*
```bash
npx serve .
# or
python -m http.server 8000
```

---

## Demo Login

- **Email / Username**: Any email (e.g. `test@example.com`)
- **Password**: Any password (8+ characters)
- Or simply click **"Sign in with Google"** for one-click access.

---

## Project Structure

```text
├── index.html        # Login & registration page
├── dashboard.html    # Main dashboard & page builder
├── css/
│   ├── style.css     # Global styles, auth design, variables
│   └── dashboard.css # Dashboard layout, cards, dark mode
├── js/
│   ├── auth.js       # Login logic & session storage
│   ├── data.js       # Sample data store
│   └── dashboard.js  # Dashboard views, charts, and drag-and-drop
└── bg.jpg / bg.png   # Background images
```

---

## Tech Stack

- **HTML5 & CSS3** (CSS Grid, Flexbox, CSS Variables)
- **Vanilla JavaScript** (ES6+)
- **Chart.js** (via CDN for charts)
- **LocalStorage** (saves your sessions, campaigns, and dark mode preference locally)

---

## Resetting Data

All campaigns and subscribers are saved in your browser's local storage. To reset to the original sample data, open your browser console (`F12`) and run:

```javascript
localStorage.clear();
location.reload();
```
