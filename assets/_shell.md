# TallUp site — shared page shell (use verbatim on every page)

Every page is a self-contained HTML file that links ONE stylesheet:
`<link rel="stylesheet" href="assets/site.css" />` (already written — do NOT modify it).

Use this exact head block (change only title/description):

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>PAGE TITLE — TallUp</title>
<meta name="description" content="PAGE DESCRIPTION" />
<link rel="icon" href="brand/icon.svg" type="image/svg+xml" />
<link rel="stylesheet" href="assets/site.css" />
</head>
<body>
```

Nav (set class="active" on the current page's link; omit `active` elsewhere):

```html
<nav class="nav"><div class="nav-inner">
  <a class="nav-brand" href="index.html"><img src="brand/icon.svg" alt="TallUp logo" /><span>TallUp</span></a>
  <div class="nav-links">
    <a href="features.html">Features</a>
    <a href="support.html">Support</a>
    <a href="privacy.html">Privacy</a>
    <a class="nav-cta" href="index.html#download">Get the app</a>
  </div>
</div></nav>
```

Footer (identical on every page):

```html
<footer class="site-footer"><div class="wrap"><div class="cols">
  <div>
    <div class="footer-brand"><img src="brand/icon.svg" alt="" /><span>TallUp</span></div>
    <p style="max-width:260px;font-size:14px;margin:0;">Stand taller every day — guided stretching, posture, sleep and nutrition habits. Not medical advice.</p>
  </div>
  <div><h4>App</h4>
    <a href="features.html">Features</a>
    <a href="index.html#premium">Premium</a>
    <a href="support.html">Support</a>
  </div>
  <div><h4>Legal</h4>
    <a href="privacy.html">Privacy Policy</a>
    <a href="terms.html">Terms of Use</a>
    <a href="delete-account.html">Delete Account</a>
  </div>
</div>
<p class="fine">© 2026 TallUp · hello@auth.tallup.app · Estimates only, based on population growth statistics — not medical advice.</p>
</div></footer>
</body></html>
```

## Assets available
- `brand/icon.svg` (app icon), `brand/lockup.svg`, `brand/mark.svg`, `brand/lockup-light.svg`
- `screenshots/01-home.png` — home dashboard with daily workout + streak
- `screenshots/02-workout-day.png` — daily workout exercise list
- `screenshots/03-player.png` — guided exercise player with timer
- `screenshots/04-progress.png` — progress charts + height check-ins
- `screenshots/05-progress-achievements.png` — achievements/badges
- `screenshots/06-nutrition.png` — sleep & nutrition tracking
- `screenshots/07-premium.png` — premium paywall
- `screenshots/08-onboarding-height.png` — onboarding height input
- `screenshots/09-onboarding-prediction.png` — adult-height prediction result

## Copy rules (mandatory)
- Product: TallUp — daily stretching/posture habit app for teens & young adults (13+).
- Core loop: 30-day plan, one guided workout/day (~10 min), 12 spine-friendly exercises, 3 difficulty levels, custom workouts, streaks.
- Prediction: personal adult-height estimate from age/height/parents' heights; ALWAYS pair with "Estimates only, based on population growth statistics — not medical advice."
- Tracking: sleep logging (8–10h goal), daily meal ideas (protein, calcium, vitamin D, zinc, magnesium), height check-ins with trend chart, achievements.
- Premium: full exercise library, custom workouts, advanced stats. Do NOT hard-code prices — write "See current pricing in the app."
- NEVER use "guaranteed to make you taller" language. Frame as habits/posture/mobility/estimates.
- Accounts are optional; app works offline, local-first.
- Download CTAs: buttons "Download on the App Store" and "Get it on Google Play" linking to "#" with a `.store-note` line "Launching soon on iOS and Android."
