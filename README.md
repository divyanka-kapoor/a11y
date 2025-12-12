# a11y+ Landing Page

AI-powered accessibility compliance platform.

## Local Development

1. Open `index.html` in a browser, or
2. Use Live Server in VS Code
3. Or run: `python -m http.server 8000`

## Deploy

- **GitHub Pages**: Push to main branch, enable Pages in Settings
- **Vercel/Netlify**: Connect repo and deploy automatically

## Backend Integration

Update the form submission in `index.html` around line 520 to connect to your backend:
```javascript
await fetch('YOUR_BACKEND_URL/api/waitlist', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email })
});
```

## Todo
- [ ] Add backend for waitlist emails
- [ ] Create privacy-policy.html
- [ ] Create terms.html
- [ ] Add analytics
```

**3. Git files:**

`.gitignore`
```
.DS_Store
*.log
node_modules/
.env