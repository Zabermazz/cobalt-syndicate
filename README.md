# Cobalt Syndicate — Official Network

A self-contained, mobile-first animated social landing page. Brand line: **Precision • Discipline • Consistency**.

## Deploy with GitHub + Vercel

1. Extract the ZIP. Create a new GitHub repository, for example `cobalt-syndicate`.
2. Choose **Add file → Upload files** and upload the **contents** of this folder. `index.html` and `vercel.json` must appear at the repository root alongside the `assets` folder. Upload extracted files, not the ZIP. Commit the files. Include `.gitignore` when using Git locally; it is not needed to render the page.
3. In Vercel, choose **Add New → Project**, connect GitHub, and import this repository.
4. Use **Framework Preset: Other**, **Root Directory: repository root (`./`)**, **Build Command: empty**, and **Output Directory: `.`**. No install command or environment variables are required. The supplied `vercel.json` already sets the framework, build and output options.
5. Click **Deploy**. Open the provided `vercel.app` address and check the social links on your phone.
6. Optional: open the Vercel project's **Settings → Domains**, add your purchased domain, and apply the exact DNS records Vercel shows at your domain registrar.

Future commits to the connected production branch trigger deployment. No domain is necessary to use the Vercel URL. Hosting plan eligibility and current pricing are controlled by Vercel.

Official guides: [Git deployment](https://vercel.com/docs/git), [build configuration](https://vercel.com/docs/builds/configure-a-build), [project configuration](https://vercel.com/docs/project-configuration/vercel-json), [domains](https://vercel.com/docs/domains/working-with-domains/add-a-domain).

## Project structure

```text
index.html              Content, metadata and all destination links
vercel.json             Static deployment configuration and security headers
README.md               Setup and maintenance
.gitignore              Keeps local secrets and generated files out of Git
assets/
  styles.css            Responsive layout, animation and reduced-motion support
  script.js             Optional motion toggle and current copyright year
  theme.css             Burgundy, ember and cream reference-inspired styling
  cobalt-logo.jpg       Original supplied Cobalt Syndicate logo
```

## Preview locally

Open `index.html` directly in a browser. There is no build, package installation or server requirement. Security headers in `vercel.json` take effect when Vercel serves the site, not when opened as a local file.

## Exact supplied destinations

| Channel / person | URL |
| --- | --- |
| Cobalt Syndicate Discord | https://discord.gg/wryHG3J9Sc |
| Telegram | https://t.me/+-NwjUdhpl11iZmY1 |
| Official X | https://x.com/cobaltsyndicat |
| Instagram | https://www.instagram.com/cobaltsyndicateofficial/ |
| YouTube | https://www.youtube.com/@CobaltSyndicateOfficial |
| Zaber | https://x.com/zaber_trades |

All external links are standard HTTPS anchors opening a new tab with `noopener noreferrer`. The official X handle intentionally retains `cobaltsyndicat` exactly as supplied. Do not add the missing-looking final "e". Telegram's `+` is part of the invite.

Link matching and local navigation can be verified independently of the platforms. Social platforms can restrict automated access; a correctly wired URL does not establish account ownership or guarantee that an invitation remains active. Keep the supplied URLs unless you have confirmed replacements. Before launch, manually confirm the Cobalt Discord and Telegram invites using your own account.

## Editing

- Change copy and links in `index.html`; the main Discord destination occurs three times (hero button, clickable hero logo and community card).
- Change base layout in `assets/styles.css` and the final colors, typography and animation in `assets/theme.css`. The theme stylesheet loads last.
- Page titles and descriptions are set in the HTML head. No invented domain or canonical URL is included. Once your final domain is connected, you may add absolute `og:url` and canonical metadata using that domain.
- Content remains visible and every link works with JavaScript disabled. The system reduced-motion setting disables animation. The page also provides a Pause motion button; that choice lasts for the current page visit.

## Privacy and maintenance

No API keys, credentials, forms, login, database, cookies, analytics, third-party fonts or third-party scripts are included. The website needs no secrets. Keep any future credentials out of the repository and out of client JavaScript. Platform privacy policies apply after visitors follow external links. Security headers are configured in `vercel.json`; adding third-party features later may require deliberate changes to the content security policy.

There are no framework dependencies to update. No deployment has been made on your behalf; this package is ready for your GitHub upload and Vercel import.

## Updated visual design

Only Cobalt Syndicate’s Discord, Telegram, X, Instagram and YouTube, plus Zaber’s X remain. Eight clickable external link placements point to six exact destinations. The supplied Cobalt artwork is used in the header, hero, community card and favicon.

Animation includes the floating logo, rotating halo, moving light and motto band. On a fine mouse pointer, a soft glow follows the pointer and cards gently tilt toward it. Touch devices keep their normal scrolling and tap behavior. All decoration is non-interactive, so links remain clickable. Pause motion and the system reduced-motion setting disable mouse effects as well as continuous animation. No cursor replacement, tracking or storage is used.
