# S-Studio — plain-language README

## What this is
A design tool that turns a written description into a picture: an infographic, social-media card, logo or poster. It can then send the result to Telegram or post it to LinkedIn.

## Who it's for
Anyone who needs quick visual content for social media or presentations.

## What it does today
- Makes four kinds of output:
  - **Animated diagrams** that build up step by step
  - **Social graphics** for Instagram or LinkedIn
  - **Logos / icons**
  - **Posters / flyers**
- Uses Google's Gemini AI to organise the content and Google's Imagen to draw the image.
- Shows a preview for you to approve before anything is sent.
- After approval, it can send the picture to a Telegram chat or post it to LinkedIn. LinkedIn posting goes through a small helper program on your own computer (`localhost:3001`).
- You type your keys into the app while using it. They are not saved in this repo.

## How to run it
This repo holds the code for one screen component, not a ready-to-open page. `index.html` actually contains React code, and there are no build settings.

To use it:
1. Create a React project with Vite (React 18).
2. Install `lucide-react`.
3. Copy the code from `index.html` into the project and show it on a page.

## Current status and known gaps
- It can't be run directly from this repo yet. It needs the setup above.
- The LinkedIn helper program is not included here.

## Where things live
| File | What's in it |
|---|---|
| `index.html` | The whole component's code |
| `README.md` | Original notes |
