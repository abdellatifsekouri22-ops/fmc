# FindMyClinic – Landing Page (Full Stack)

A desktop-first landing page closely matching the screenshots, with a simple Node/Express backend to capture leads.

## Quick start
```bash
# 1) Install deps
npm install

# 2) (Optional) copy .env.example to .env and fill SMTP_* + NOTIFY_TO for email notifications
cp server/.env.example server/.env

# 3) Run
npm run dev

# Open http://localhost:8080
```

### Project structure
```
findmyclinic-site/
├─ frontend/
│  ├─ index.html
│  ├─ script.js
│  └─ assets/logo.svg
└─ server/
   ├─ server.js
   ├─ .env.example
   └─ leads.json (auto-created)
```

The frontend uses Tailwind via CDN for speed. For production, compile Tailwind and minify assets.

## Notes
- The WhatsApp link in the header/footer is a placeholder; replace with your number in `index.html`.
- The country list is a quick subset; extend it as you like in `script.js`.
- The backend stores submissions to `server/leads.json` and (optionally) emails them.
