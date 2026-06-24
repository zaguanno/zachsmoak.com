# zachsmoak.com

Personal portfolio site built with [Hugo](https://gohugo.io) + [CareerCanvas](https://github.com/felipecordero/careercanvas) theme. Deployed to Firebase Hosting via GitHub Actions on every push to `main`.

## Local development

```bash
npm install
hugo server -D
```

Site runs at `http://localhost:1313`.

## Deployment

Push to `main` → GitHub Actions builds Hugo → deploys to Firebase automatically. No manual steps.

---

## Dashboards & consoles

| Service | Purpose | Link |
|---|---|---|
| **Firebase Hosting** | Live site, custom domain, deploy history | [console.firebase.google.com/project/zachsmoak-site/hosting](https://console.firebase.google.com/project/zachsmoak-site/hosting) |
| **Google Cloud Console** | IAM, service accounts, API keys | [console.cloud.google.com/home/dashboard?project=zachsmoak-site](https://console.cloud.google.com/home/dashboard?project=zachsmoak-site) |
| **GitHub Actions** | Build & deploy pipeline, run history | [github.com/zaguanno/zachsmoak.com/actions](https://github.com/zaguanno/zachsmoak.com/actions) |
| **GitHub Secrets** | `FIREBASE_SERVICE_ACCOUNT` key management | [github.com/zaguanno/zachsmoak.com/settings/secrets/actions](https://github.com/zaguanno/zachsmoak.com/settings/secrets/actions) |
| **Formspree** | Contact form submissions & notifications | [formspree.io/forms](https://formspree.io/forms) |
| **Google Calendar** | Appointment scheduling link | [calendar.google.com](https://calendar.google.com) |
| **Squarespace DNS** | zachsmoak.com domain & DNS records | [account.squarespace.com/domains](https://account.squarespace.com/domains) |

## Key config locations

| What | Where |
|---|---|
| Site-wide settings, colors, social links | `hugo.toml` |
| Nav menu items | `config/_default/menus.en.toml` |
| Hero, About, Skills, Experience, Technical content | `content/en/` |
| Layout overrides (nav, footer, hero, experience, contact) | `layouts/partials/` |
| Custom CSS (hero dark mode isolation) | `assets/css/custom.css` |
| Resume PDF | `static/files/ZSmoak_Resume_v7.1.pdf` |
| Profile photo & favicons | `static/images/` |
| Firebase hosting config | `firebase.json`, `.firebaserc` |
| CI/CD pipeline | `.github/workflows/deploy.yml` |
