# 🌍 YourWorld — Stories, Creative Studio, Private Sharing & PDF Tools

YourWorld is a web platform for creating visual stories, organizing files, making creative projects, and sharing work with controlled access. It brings a multi-page story canvas, file previews, AI-assisted creation, a private vault, a browser-based PDF editor, and a creative Studio together under one product.

**Live product:** [https://worldbyyou.com](https://worldbyyou.com/)

> **About this repository:** This is a public portfolio and product overview. It intentionally contains this README only; the production application source, deployment configuration, and credentials are maintained privately. This repository is not a downloadable or self-hostable version of YourWorld.

---

## Contents

- [The problem and the approach](#-the-problem-and-the-approach)
- [Product areas](#-product-areas)
  - [Story canvas and sharing](#1-story-canvas-and-sharing)
  - [PDF editor](#2-pdf-editor)
  - [Studio](#3-studio)
  - [Files, previews, and Private Vault](#4-files-previews-and-private-vault)
  - [Aura AI and creative tools](#5-aura-ai-and-creative-tools)
  - [Accounts and plans](#6-accounts-and-plans)
- [Typical workflows](#-typical-workflows)
- [Usability, accessibility, and reliability](#-usability-accessibility-and-reliability)
- [System architecture](#-system-architecture)
- [Technology overview](#-technology-overview)
- [Performance and reliability work](#-performance-and-reliability-work)
- [Privacy and security](#-privacy-and-security)
- [Validation approach](#-validation-approach)
- [Project goals and impact](#-project-goals-and-impact)
- [Author](#-author)

---

## 🎯 The problem and the approach

Writing, file storage, creative editing, PDF updates, and private sharing often happen in separate tools. Moving between them makes it harder to keep related content together, preview what another person will see, and control whether a recipient can edit or only view.

YourWorld connects these workflows. A user can create a story from pages, attach media, preview supported files, personalize the experience, and share selected work. Separate tools support PDF annotations and visual replacements, while Studio provides a creative editing workspace.

---

## ✨ Product areas

### 1. Story canvas and sharing

The story canvas is a multi-page workspace for writing and arranging content.

- **Write and format:** Create pages with rich text and adjust formatting as you compose.
- **Organize pages:** Add pages, move them into the desired order, and continue a story across multiple pages.
- **Add media and files:** Attach images and supported files to bring related material into the story.
- **Personalize:** Choose visual themes and, where available, ambient audio or custom songs.
- **Preview:** Open a story in its viewer before sharing it, so the recipient experience can be checked.
- **Present:** Use slideshow mode to move through story pages as a presentation.
- **Export:** Use the available PDF or download workflows to produce a portable copy.

#### Share codes and permissions

Sharing is designed around choosing what to share and what recipients may do.

- Create generated codes or choose a custom code where available.
- Share a full canvas or selected pages in supported workflows.
- Set a shared story to view-only or allow editing, depending on the workflow.
- Update or remove active codes and manage the current share access.
- Open a shared story through its viewer without exposing the private application repository.

The share-code system connects a code to the intended story or pages and their access mode. YourWorld also includes Quick Share for temporary file handoffs; its available limits and expiry depend on the current product plan and settings.

### 2. PDF editor

The browser-based **Edit PDF** tool supports common visual updates and annotations without requiring a desktop PDF application.

#### Add and annotate

- Add text and position it on a page.
- Insert images and signatures.
- Draw freehand marks, add highlights, and place common shapes such as rectangles, circles, lines, and arrows.
- Adjust text appearance, including font family, size, color, bold, italic, underline, and alignment where supported by the selected editing tool.
- Move and rotate editable text objects and annotations.
- Use undo and redo for supported editing actions.
- Review the page in the editor before exporting the updated PDF.

#### Replace visible text

Visual text replacement helps update items such as names or dates while preserving the surrounding page appearance as closely as practical.

- Select detected text and enter replacement text.
- Apply font, size, color, background cover color, alignment, and style choices.
- Format selected characters independently when the replacement editor supports a text selection; with no character selection, formatting applies to the whole replacement.
- Position or rotate the replacement to fit the page.
- Inspect the live preview and final page before export.

Text replacement is a visual edit: it covers the original printed area and places new text over it. It does not guarantee reconstruction of the PDF's original underlying text objects or exact font metrics. Font availability, source layout, and replacement length can affect the result, so review exported pages before relying on them.

#### Scanned documents and OCR

OCR-assisted detection can recognize text on supported scanned pages so that text regions can be selected for editing. Recognition quality and speed depend on scan clarity, page orientation, language, device, and document size. OCR is a helper for finding text; review its result and the exported PDF.

#### Upload and export

Open a PDF using the file picker or drag-and-drop onto the supported editor upload area. Make edits in the page workspace and export the resulting PDF when ready. Export behavior depends on the source PDF and the features used; inspect the saved file to confirm page layout and annotations.

### 3. Studio

**Studio** is YourWorld's creative editing area for assembling visual projects from media and design elements. It is intended for creating short compositions and exporting a finished result.

Depending on the project and browser capabilities, Studio includes:

- A multi-track timeline for arranging video, audio, text, and image or overlay clips.
- A preview canvas for checking composition and playback.
- Text and title presets, templates, overlays, shapes, GIF-style stickers, and other creative elements.
- Controls for moving, trimming, splitting, duplicating, and deleting timeline clips.
- Transform, opacity, text appearance, color adjustment, and effect controls.
- Audio and video playback controls, including volume and speed where supported.
- Undo and redo, autosaving, and project recovery in the browser.
- Export settings for video resolution, frame rate, and encoding where supported by the browser and device.

Studio's media editing and video export capabilities are browser-dependent. Export options can vary by device, browser, memory, and media format. Studio is a separate creative tool within YourWorld; it is not the same editor as the story canvas or PDF editor.

### 4. Files, previews, and Private Vault

YourWorld supports file workflows around stories and sharing:

- Upload files through supported pickers and drag-and-drop upload areas.
- Preview supported formats inside the product before opening or downloading them.
- Share files through supported Quick Share workflows.
- Store saved work in the **Private Vault** when signed in.
- Access files through generated or custom share codes where supported.

Preview support varies by file type. A preview is intended to make it easier to inspect content; it does not replace the original file or guarantee that every format behaves identically across browsers.

### 5. Aura AI and creative tools

Aura AI helps users work with story content through writing assistance, such as drafting, rewriting, editing, and brainstorming. AI image generation can create visual assets for supported story workflows. Themes, media, and creative tools help users shape a story's presentation.

AI features depend on the current service configuration, plan limits, and availability. Generated results should be reviewed before sharing or publishing.

### 6. Accounts and plans

Signed-in product areas support account settings, saved content, activity information, and plan-related workflows. Some capabilities have plan-based limits or eligibility. Current availability is shown in the live product and may change over time.

---

## 🔁 Typical workflows

### Create and share a story

**Create pages → write and add media → choose a theme → preview as a viewer → select sharing access → send the code**

### Edit a PDF

**Open or drop a PDF → annotate or visually replace text → inspect the page preview → export → review the saved PDF**

### Make a Studio project

**Start a project → add media and design elements → arrange and edit the timeline → preview → export in a supported format**

### Share a file

**Upload a supported file → check its preview → select the available sharing option → share the link or code**

---

## 📱 Usability, accessibility, and reliability

YourWorld is maintained for desktop and mobile use. Editing interfaces adapt to smaller screens, with controls and previews intended to remain usable on touch devices as well as with a mouse and keyboard.

Ongoing product work includes:

- Keeping the story canvas, viewer, PDF editor, and Studio usable at different screen sizes.
- Making upload actions easier to discover, including drag-and-drop in supported areas.
- Providing previews before users finalize edits or exports.
- Improving text selection and formatting behavior in the PDF replacement workflow.
- Addressing issues found in editing, sharing, file handling, and export.
- Improving error handling so that expected document or export problems can be reported clearly.

---

## 🏗️ System architecture

At a high level, the production system follows this flow:

```text
Browser
  ├── Story canvas, viewer, PDF editor, Studio, Vault, and product pages
  ├── JavaScript interactions and in-browser document/media rendering
  └── Authenticated or public requests
        ↓
Flask application
  ├── Page and authentication routes
  ├── Canvas, story, and share-code APIs
  ├── File upload, preview, and download APIs
  ├── AI and creative-service routes
  ├── User, settings, and billing routes
  └── Payment webhook handling
        ↓
Firestore + object storage + AI providers + payment provider
```

The server renders product pages and provides APIs for data, sharing, accounts, and file workflows. The browser provides interactive editing and previews. Private application source and deployment configuration are intentionally not published in this repository.

---

## 🧰 Technology overview

The private production application uses a web stack that includes:

- **Backend:** Python and Flask, served with Gunicorn.
- **Page rendering:** Jinja templates.
- **Frontend:** HTML, CSS, and JavaScript for the main product UI and interactive editing tools.
- **Data:** Firebase Admin and Firestore for application records.
- **File storage:** Cloudflare R2 using the S3-compatible API.
- **PDF and media workflows:** Browser rendering and editing libraries, with server-assisted processing for supported tasks.
- **AI services:** Provider integrations for text assistance and image generation.
- **Payments:** Razorpay integration for supported plan flows.
- **Production delivery:** Nginx and systemd on VPS infrastructure.

The standalone Studio editor has its own TypeScript and React-based frontend and uses browser media APIs for editing and export. This is a high-level overview, not a dependency list or installation guide.

---

## ⚡ Performance and reliability work

Work on performance and correctness includes improvements to:

- **Share-code updates:** Keep the active code for a story/share combination consistent when a code is regenerated or customized.
- **Permission updates:** Improve the responsiveness of view/edit permission changes and batch related backend writes where appropriate.
- **Lookup behavior:** Use direct code lookups for relevant operations instead of unnecessarily scanning records.
- **Editing history:** Provide undo/redo for supported story, PDF, and Studio editing actions.
- **Document handling:** Improve OCR reuse and editor state restoration for supported PDF workflows.
- **Export handling:** Validate inputs and report supported failures during PDF and media export instead of leaving users with an unexplained result.
- **Interface behavior:** Fix interaction and responsive-layout issues found during desktop and mobile use.

These are continuing engineering efforts; actual speed depends on the network, document size, device, browser, and external service availability.

---

## 🔐 Privacy and security

The public showcase deliberately excludes production source code, user data, database exports, API keys, payment secrets, and deployment credentials.

The production product uses authenticated workflows for account-specific features and scoped access for shared content. Public viewing is limited to content exposed through its sharing workflow. Private routes and user data are not intended as public content. Payment events use server-side webhook handling.

File processing varies by feature: PDFs are opened in the browser where supported, while OCR or server-assisted download flows may use temporary processing. Users should consult the live site's privacy policy for current file-handling details.

---

## ✅ Validation approach

The private application is developed with automated checks for important product paths. Coverage includes areas such as:

- Story editing, saving, and sharing flows.
- Share-code creation, updates, permission changes, and removal.
- Public story viewing and authenticated editing.
- File previews, upload interactions, and slideshow/PDF workflows.
- PDF replacement, formatting, placement, OCR-assisted pages, undo/redo, and export behavior.
- Studio editing and browser-based media export behavior.

Automated checks complement manual review across screen sizes and browsers. PDF fonts, OCR output, and media exports still need visual or playback review because source documents and browser capabilities vary.

---

## 🌱 Project goals and impact

YourWorld explores how a single product can connect:

- Story creation and visual presentation.
- Private sharing with explicit access choices.
- File organization and previews.
- AI-assisted writing and image creation.
- Practical document edits and creative media workflows.
- Browser-based tools that work across desktop and mobile.

It is also a full-stack product project spanning interface design, backend APIs, storage, authentication, AI integrations, payment flows, privacy boundaries, and production operations.

---

## 📌 Repository notes

- This repository is a public README-only overview.
- The production application's source code is private.
- There is no runnable app, Docker image, or self-hosting setup in this repository.
- To explore the product, use the [live YourWorld site](https://worldbyyou.com/).

---

## 👨‍💻 Author

Built by [Dhruva Gowda](https://github.com/DhruvaGowda-Coder).
