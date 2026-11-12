# Dobby Design

A weaving draft and design editor that runs entirely in the browser. No build step, no server, no packages to install. It can be installed on a phone, tablet or computer like an app.

## What it does

- Threading, tie-up, treadling and peg plan, with a live draw-down
- A Design pane that is always linked to the draft and peg plan: change either side and the other follows
- Drag across the design to select a range, click a cell to flip it
- Denting row and reed count (dents per 2 inches)
- Weave library with 50+ weaves, plus your own saved weaves
- Repeat, mirror, duplicate, colour ranges and stripes
- WIF and JSON import and export
- Print sheet with the peg plan, drawing-in sequence, denting and colours

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app. This is the only file you change when you update Dobby Design. |
| `manifest.webmanifest` | Name, colours and icons used when the app is installed. |
| `sw.js` | Lets the app open offline. It loads the newest `index.html` whenever you are online. |
| `icons/` | The Dobby Design logo in the sizes phones, tablets and browsers need. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are. |

Upload all of them once. After that, an update is just a new `index.html`.

## Put it online with GitHub Pages

1. Create a new repository on GitHub, for example `dobby-design`.
2. Upload everything in this folder, including the `icons` folder and `.nojekyll`.
3. Open Settings, then Pages. Under Build and deployment choose Deploy from a branch, branch `main`, folder `/ (root)`, and Save.
4. After a minute the app is live at `https://YOUR-USERNAME.github.io/dobby-design/`.

Installing needs the secure `https` address, which GitHub Pages gives you.

## Install on a device

- **Chrome or Edge on Windows, Mac, Linux, Android:** open the page, then use the install icon in the address bar, or the browser menu, Install app. Inside the app you can also use the ? menu, Install on this device.
- **iPhone or iPad (Safari):** tap Share, then Add to Home Screen.

The installed app opens in its own window with the Dobby Design icon and works offline.

## Your data

Drafts and saved weaves are stored in the browser or installed app on that device (localStorage). They are not in the repository. Use File, Import and export, then Export JSON (or Copy my weaves in the Weave library) to keep a copy or move to another device.

## Print

File, Print sheet builds an image of the draft, peg plan, drawing-in sequence and denting. Save the image, then print it.
