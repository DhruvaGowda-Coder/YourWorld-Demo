# YourWorld

YourWorld is an AI-powered storytelling and shared canvas platform for creating rich, interactive story spaces with pages, media, private vault storage, smart sharing, and AI-assisted creation.

Live demo: [worldbyyou.com](https://worldbyyou.com)

> This public repository is a portfolio/demo overview. The production source code is private because YourWorld is a startup/proprietary project.

## What It Does

YourWorld helps users create a personal or collaborative story canvas where text, images, files, generated media, and shareable pages can live together in one polished experience.

Core capabilities include:

- Story canvas with multiple pages
- Rich text and media editing
- AI-assisted writing and image generation
- Aura AI assistant for story guidance and creation help
- Vault for storing uploaded files and generated assets
- Quick Share for temporary file/page sharing
- Custom share codes and generated share codes
- Permission control for view-only and edit-enabled sharing
- Smart previews for shared content
- PDF/download-oriented sharing workflows
- Slideshow-style story viewing experience
- Theme and custom audio personalization
- User account settings and activity tracking
- Payment/subscription-ready user flows
- Secure deployment on a production VPS

## Why I Built It

I built YourWorld to combine creative storytelling, AI generation, file organization, and real-time sharing into one focused product experience. The goal was to make a canvas that feels personal enough for creative work, but structured enough to share with others through controlled links and codes.

## Demo Highlights

- Create a story with multiple pages
- Add text, media, uploads, and generated images
- Generate a share code or set a custom share code
- Choose whether others can view or edit
- Share selected pages or the full canvas
- Store and reuse files through the vault
- Use Aura AI for creative assistance
- Preview and share content without exposing private user data

## Tech Stack

The private production app uses:

- Python
- Flask
- Jinja templates
- Vanilla JavaScript
- HTML/CSS
- Firebase/Firestore-style document storage
- Cloud object storage for uploaded files
- AI image/text generation integrations
- Razorpay-style payment flow integration
- Nginx + systemd production deployment
- VPS hosting

## Architecture Overview

The app is organized around a Flask backend with route modules for:

- public pages and story viewing
- canvas and share-code APIs
- file upload and preview APIs
- AI chat and image generation
- user settings, billing, and account activity
- payment webhooks

The frontend is built with server-rendered templates and focused JavaScript modules for the editor, chat assistant, file handling, previews, and share controls.

## Performance Work

The share-code system was optimized so common actions are faster and more reliable:

- generated code replaces the previous active code for the same story/share combination
- custom code replaces the previous generated code instead of leaving duplicate active codes
- delete active removes the active code cleanly
- edit/non-edit permission updates are debounced for faster user feedback
- backend writes for share-code updates are batched where possible
- lookup updates are handled directly instead of relying on slower scans

Recent testing showed the slowest share-code operations were reduced significantly compared with the earlier version, especially custom-code replacement and duplicate-code handling.

## Security And Privacy

This public repository intentionally does not include:

- production source code
- API keys
- Firebase credentials
- payment secrets
- deployment credentials
- database structure exports
- private business logic
- user data

The production app is designed with authenticated user flows, scoped sharing, permission checks, and private data boundaries.

## Testing

The private project includes automated backend and browser tests covering major flows such as:

- share-code creation
- custom-code replacement
- duplicate-code protection
- edit permission updates
- delete active share code
- payment/security behavior
- public story viewing
- authenticated story editing

## Current Status

YourWorld is live as a working product demo and is actively maintained as a private startup project.

Live demo: [worldbyyou.com](https://worldbyyou.com)

## Author

Built by [Dhruva Gowda](https://github.com/DhruvaGowda-Coder).
