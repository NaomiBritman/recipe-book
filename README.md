# My Recipe Book

A recipe web app that reads cooking instructions aloud, step by step, so you can follow a recipe without touching the screen. Built with plain HTML, CSS and JavaScript, with no frameworks and no build step.

## Features

- Sign up and log in, with a separate settings profile per user
- Browse recipes as cards and search them
- Add your own recipes, including an image upload with preview
- Recipe view with ingredients and numbered steps
- **Read aloud:** the browser reads each step using the Web Speech API, with start, pause, resume and stop controls
- Settings per user: delay between steps, voice, reading speed, and light or dark theme
- Hebrew, right-to-left interface
- All data is stored in the browser with `localStorage`

## Tech stack

- HTML5 and CSS3
- Vanilla JavaScript
- Web Speech API (`speechSynthesis`)
- `localStorage` for persistence

## Project structure

```
├── index.html            # Landing page with image slider
├── login.html            # Log in
├── signup.html           # Sign up
├── recipes.html          # Recipe list, search, add recipe
├── recipe_view.html      # Single recipe with read-aloud controls
├── settings.html         # User settings
├── css/styles.css
├── images/
└── js/
    ├── data-manager.js       # Storage layer: users, recipes, settings
    ├── speech-reader.js      # Step-by-step text-to-speech
    ├── recipes-app.js        # Recipe list page
    ├── recipe-view-app.js    # Recipe page
    ├── login-handler.js
    ├── signup-handler.js
    ├── settings-handler.js
    └── slider.js
```

## Getting started

No installation is needed.

1. Clone the repository.
2. Open `index.html` in a browser, or serve the folder with any static server.
3. Sign up, or log in with the demo user `guest` / `guest`.

Reading aloud needs a browser that supports speech synthesis, and a Hebrew voice installed for Hebrew recipes.

## Notes

This is a front-end demo project. Accounts live only in the browser's `localStorage`, so it is not meant for real user data.
