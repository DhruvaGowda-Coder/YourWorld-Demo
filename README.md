# 🌍 YourWorld — AI Storytelling & Private Sharing Workspace

<p align="center">
  <img src="https://worldbyyou.com/static/img/yourworld-symbol.png" alt="YourWorld logo" width="120" />
</p>

YourWorld is an AI-powered storytelling and shared canvas platform for creating rich, interactive story spaces with pages, media, private vault storage, smart sharing, and AI-assisted creation.

> This public repository is a portfolio/demo overview. The production source code is private because YourWorld is a startup/proprietary project.

---

## 🌐 Live Demo

👉 https://worldbyyou.com/

---

## 🎯 Problem Solved

Creators and teams often need one place to write stories, store files, generate creative assets, preview content, and share selected pages with controlled access.

Most workflows force users to jump between notes apps, file drives, AI tools, PDF exporters, and link-sharing tools.

---

## 💡 Solution

YourWorld brings story creation, private sharing, smart previews, AI assistance, image generation, vault storage, PDF/slideshow workflows, and edit permissions into one clean web experience.

Users can build a story canvas, add files and media, personalize it with themes, and share it using generated or custom codes.

---

## ✨ Key Features

* Story canvas with multiple pages
* Rich text and media editing
* AI-assisted writing and image generation
* Aura AI assistant for story guidance and creation help
* Vault for storing uploaded files and generated assets
* Quick Share for temporary file/page sharing
* Custom share codes and generated share codes
* Permission control for view-only and edit-enabled sharing
* Smart previews for shared content
* PDF/download-oriented sharing workflows
* Slideshow-style story viewing experience
* Theme and custom audio personalization
* User account settings and activity tracking
* Payment/subscription-ready user flows
* Secure VPS deployment

---

## 🧠 How It Works

Story Input → Canvas Pages → Files / AI / Themes → Share Code → Viewer / Editor Permissions → Smart Preview, PDF, or Slideshow

---

## 🏗️ Tech Stack

* **Backend**: Python, Flask
* **Templates**: Jinja
* **Frontend**: Vanilla JavaScript, HTML, CSS
* **Database**: Firestore-style document storage
* **Storage**: Cloud object storage
* **AI**: Text and image generation integrations
* **Payments**: Razorpay-style payment flow
* **Production**: Nginx, systemd, VPS hosting

---

## 🧩 Architecture

Flask Backend → Route Modules → Database + Storage + AI + Payments → Server-Rendered UI → JavaScript Editor → Public Viewer / Vault / Story Workspace

The production app is organized around route modules for:

* Public pages and story viewing
* Canvas and share-code APIs
* File upload and preview APIs
* AI chat and image generation
* User settings and account activity
* Billing and payment webhooks

---

## ⚡ Performance Work

The share-code system was optimized so common actions are faster and more reliable:

* Generated code replaces the previous active code for the same story/share combination
* Custom code replaces the previous generated code instead of leaving duplicate active codes
* Delete active removes the active code cleanly
* Edit/non-edit permission updates are debounced for faster user feedback
* Backend writes for share-code updates are batched where possible
* Lookup updates are handled directly instead of relying on slower scans

---

## 🔐 Security & Privacy

This public repository intentionally does **not** include:

* Production source code
* API keys
* Firebase credentials
* Payment secrets
* Deployment credentials
* Database exports
* Private business logic
* User data

The production app is designed with authenticated user flows, scoped sharing, permission checks, private data boundaries, and secure deployment practices.

---

## ✅ Testing

The private project includes automated backend and browser tests covering major flows such as:

* Share-code creation
* Custom-code replacement
* Duplicate-code protection
* Edit permission updates
* Delete active share code
* Payment/security behavior
* Public story viewing
* Authenticated story editing

---

## 📌 Notes

* Public demo repository contains only the project overview
* Production code is private to protect the startup/product
* Live product is deployed and actively maintained
* README is designed for recruiters, resume review, and portfolio visitors

---

## 🎯 Impact

* Combines AI, storytelling, file sharing, previews, and permissions in one platform
* Shows full-stack product thinking across frontend, backend, AI, payments, and deployment
* Demonstrates real-world private sharing workflows with custom access codes
* Gives users a creative workspace that can become a story, vault, slideshow, or shareable page

---

## 👨‍💻 Author

Built by [Dhruva Gowda](https://github.com/DhruvaGowda-Coder).
