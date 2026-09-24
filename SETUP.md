# 🔌 Connect Guide

Every dynamic piece of this profile README, how to switch it on, and what to do once everything is live.
Total time to 100%: **about 25 minutes**, all free, no credit card anywhere.

| # | Thing | Time | Needs an account? | Needs a deploy? |
|---|-------|------|-------------------|-----------------|
| 1 | Profile README visibility (repo rename) | 2 min | — | — |
| 2 | 🐍 Snake animation | 1 min | — | — |
| 3 | Social link badges | 2 min | — | — |
| 4 | ⏱️ WakaTime coding hours | ~10 min | ✅ WakaTime (free) | ❌ |
| 5 | 🎧 Spotify now playing | ~2 min | ✅ Spotify (free tier is fine) | ❌ |
| 6 | Final polish checklist | 5 min | — | — |

---

## 1 · Make the README actually appear on your profile (2 min)

GitHub only shows a profile README from a repository **named exactly like your username**.
This repo is still `Oluwadaredaniel` (from before the rename), so:

1. Repo → **Settings → General → Danger Zone → Rename** → `Emerald-dev0`.
2. Back in `README.md`, search for `Oluwadaredaniel` and update the **two snake URLs** (a comment marks the spot).

## 2 · Snake (1 min)

Repo → **Actions** tab → workflow **"🐍 Snake"** → **Run workflow**.
After that it re-runs automatically every 12 hours and on every push to `main`.

## 3 · Social badges (2 min)

In `README.md` search for `EDIT ME` in the **Let's Connect** section and replace the `#` / placeholder hrefs
with your real X, LinkedIn and email links.

## 4 · ⏱️ WakaTime coding hours (~10 min)

WakaTime quietly tracks which languages/editors you code in, straight from your editor.

1. **Sign up** at [wakatime.com](https://wakatime.com) (the "Sign up with GitHub" button is easiest).
2. **Install the plugin** for your editor — in VS Code: Extensions → search **WakaTime** → Install → sign in when prompted.
   (There are plugins for JetBrains, Neovim, Sublime, and a CLI for terminal work.)
3. **Go public:** WakaTime → **Settings → Profile** → turn on **"Publicly display my coding activity"**
   (wording may read "Display my coding activity publicly"). Without this the card can't fetch your stats.
4. **Code for a bit.** Stats appear after the plugin sends its first heartbeats (usually within minutes).
5. In `README.md`, in the **Where The Hours Go** section, replace both `EDIT_ME` occurrences in the card URL
   with your WakaTime handle (the `@something` on your profile, without the `@`).
6. Delete the "⏳ Wiring in progress" line under the card.
7. Test: paste the card URL into a browser tab — you should see your emerald stats card, not an error.

> Free tier is plenty. The card shows this week's hours split by language — it updates by itself forever.

## 5 · 🎧 Spotify now playing (~2 min)

**Yes, this one needs your Spotify account connected — but it's a single click, no code, no deploy,
no Spotify Developer app, and Premium is NOT required.** The [spotify-github-profile](https://github.com/kittinan/spotify-github-profile)
project runs a free hosted service that stores only your tokens and renders the badge.

1. Open **<https://spotify-github-profile.kittinanx.com/api/login>** and click **Connect with Spotify**.
   Approve the permission screen (it only reads what's currently playing — it cannot control playback).
2. After connecting you'll see your **uid** — copy it.
3. In `README.md`, in the **Now Spinning** section, replace `EDIT_ME` in the badge URL with your uid.
4. Delete the "⏳ Wiring in progress" line under the badge.
5. Play something and refresh your profile — album art, track and an equalizer bar appear. When nothing is
   playing it shows a tasteful "offline" state (`show_offline=true`); set it to `false` if you'd rather hide that.

> Want it fully self-hosted later (your own Vercel + Firebase, zero third parties)? The project README has
> the full self-host path — say the word and I'll set it up in this repo.

## 6 · Final polish — "everything is connected, what next?" (5 min)

Once the widgets are live, these are the highest-impact moves left, in order:

1. **Pin 6 repos** on your profile page (profile → "Customize your pins") — pick Calder, Blueprint, LIFELINK,
   AOT, Portfolio, Noma-Form. Pins + README are the one-two punch visitors see first.
2. **Add topics to your repos** (`typescript`, `react`, `nextjs`, `ai`…) — topics make repos discoverable in
   GitHub search and make the top-langs/trophy cards richer over time.
3. **Write one-line descriptions** for any repo still missing one (several currently show blank).
4. **Star your own favourite repos? No — star other people's.** A curated star list reads as taste; also
   follow devs you admire. Both feed the trophy card.
5. **Portfolio cross-link:** put the GitHub URL in your portfolio footer and the portfolio URL in your GitHub
   profile "Links" field (profile → Edit profile) so the two amplify each other.
6. **Keep the snake fed:** the only maintenance this README needs is… committing. Everything else is automated.

### Optional extras I can wire in whenever you want

- 🏆 **LeetCode / Chess.com / Codewars** stat cards (if you grind there)
- 📝 **Latest blog posts / dev.to articles** — auto-updating list via RSS
- 🎬 **YouTube latest videos** card
- 💻 **Animated terminal session** (recorded with VHS/asciinema, embedded as GIF)
- 🌐 **Social preview images** for your repos (og-image banners via socialify)
- 🗺️ **3D contribution graph** render

Just ask and I'll add the section + guide entry.

---

### FAQ

- **Does any of this cost money?** No. WakaTime free tier, Spotify free tier, hosted badge services free, GitHub Actions free for public repos.
- **Is the Spotify connection safe?** It grants read-only "now playing" scope to an open-source service; tokens are stored for refresh only. Self-host option exists if you're strict about it.
- **Will the cards work while my repo is still named `Oluwadaredaniel`?** The cards work anywhere the markdown renders — but the README only shows *on your profile page* after the rename in §1.
- **Something shows an error card?** 99% of the time it's a wrong username/uid or WakaTime privacy still private. Open the image URL in a tab — the error message tells you which.
