# S-Studio

A single-file React component that turns a text prompt into visual content — infographics,
social cards, logos, and posters — then publishes the result to Telegram or LinkedIn.

## What it generates

| Type | Output |
|---|---|
| Consultant Architect | Phased, narrative-driven animated data architectures drawn on a canvas |
| Social Graphic | Instagram / LinkedIn card |
| Logo / Icon | Vector-style mark |
| Poster / Flyer | Visual mockup |

## How it works

1. You describe what to architect.
2. The component calls the Gemini API to structure the content and Imagen to render the image.
3. The result is previewed on an animated canvas for approval.
4. Once approved it can be sent to a Telegram chat or posted to LinkedIn.

## External services

| Service | Endpoint | Purpose |
|---|---|---|
| Google Gemini | `generativelanguage.googleapis.com` | Content structuring and image generation |
| Telegram Bot API | `api.telegram.org` | Draft preview and approval flow |
| LinkedIn proxy | `localhost:3001/api/linkedin` | Posting, via a local proxy |

API keys and tokens are entered in the UI at runtime and are not stored in the repository.

## Status

This repository holds source, not a runnable page. `index.html` contains JSX rather than an HTML
document, and no build configuration is checked in. To run it, add the component to a React +
Vite project (React 18, `lucide-react`) and mount it.

## Layout

| Path | Purpose |
|---|---|
| `index.html` | The component source |
| `README.md` | This file |
