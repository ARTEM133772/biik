# Biik: exam preparation for students in Kazakhstan

Biik is a paid web app that prepares school students in Kazakhstan for the ENT, the national university entrance exam that decides state grants, and for IELTS. Built in Astana since September 2026.

**Site:** https://biik.kz (in Russian) · **English summary:** https://biik.kz/about

## What it does

- A daily study plan built from the learner's own weak task types.
- 227 short explainer videos, one per topic, with every word shown on screen.
- A question bank checked on the server; answer keys never reach the browser.
- A monthly mock exam in the official format and a free diagnostic test.
- Mistakes come back on days 1, 3 and 7 until they stick.
- A weekly league by city, duels with friends, and a Telegram reminder bot.

## How a learner uses it

1. Sign up, take a 30-question diagnostic, and get a first score forecast.
2. Study the daily plan: short videos, tasks, and an AI tutor that explains wrong answers.
3. Take the monthly mock exam; a parent follows progress through a private link.

## AI in Biik

The in-app tutor explains wrong answers, checks typed and photo answers, and reads tasks aloud. Today it runs on Google Gemini. The product itself, including about 300 automated tests, is written with Claude Code.

## Safety for students

- The tutor is instructed to stay on study topics; a photo is described before it is discussed.
- Questions written by AI are solved a second time blind and kept only if both answers match; they are labelled and can be removed.
- Every task has a "report an error" button.
- Signup records consent; for learners under 18 a parent gives it.
- Account and data are deleted on request within 7 days.

## How it is built

Next.js on Cloudflare Workers, files in Cloudflare R2. The `.kz` domain zone requires a server inside Kazakhstan, so visitors reach the site through a small server in Almaty that passes requests on. The source code lives in a private repository; this page is the public description of the product.

## Pricing

Three free days, then 4 990 KZT a month for Start or 9 990 KZT for Pro. Full pricing: https://biik.kz/prices (in Russian).

## Team

Biik is built by a two-person family team in Astana, Kazakhstan, with no outside funding. Our first paying learner joined during the closed test; public launch is 12 October 2026.

## Contact

Support runs through the Telegram bot [@biik_remind_bot](https://t.me/biik_remind_bot?start=help).
