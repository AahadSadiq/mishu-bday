# Happy Birthday Navya 

A pink retro Game Boy-style birthday website. Open `index.html` in a browser to preview it.

## Add the birthday videos
1. Put each MP4 in the `videos/` folder.
2. Open `index.html` and find `const FRIEND_VIDEOS`.
3. Replace the sample names and filenames with the real names and exact filenames.
4. Add or remove entries as needed. The gallery creates one card per entry.

Example:
`{ name: "Aahad", caption: "Your favourite menace", file: "aahad.mp4" }`

Use reasonably compressed MP4 (H.264) files. For GitHub Pages, keep the total repository size manageable; large videos are better hosted elsewhere and linked via a direct video URL.

## Personalise the quiz
In `index.html`, find `const QUIZ_QUESTIONS`. Replace the sample questions with Navya-specific inside jokes and facts. `answer` is zero-based: 0 = first option, 1 = second, etc. Use exactly four options per question.

## Add photos
The memory section is currently a six-tile placeholder. Add your photos to `photos/`; the next step is to wire those exact filenames into the gallery. (The folder is included so you can drop them in.)

## Publish with GitHub Pages
1. Create a new public GitHub repository, e.g. `navya-birthday`.
2. Upload `index.html`, plus the `videos` and `photos` folders.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select **main** and **/(root)**, then Save.
6. Wait for GitHub to publish the site. The URL will look like `https://YOUR-USERNAME.github.io/navya-birthday/`.

Keep the birthday videos private if that matters to your group: a public GitHub Pages site and public repository are not appropriate for sensitive videos. Consider hosting videos privately or using a private sharing setup.

## Opening-screen bouncing cousin faces
The opening screen now uses `photos/mishu-sprite.png`. It contains the supplied cousin photo with its birthday hat. The faces bounce around the pink stage, sparkle on wall impacts, and show **HAPPY BIRTHDAY MISHU!** when clicked. The animation is built into `index.html`; no extra setup is needed.

Before publishing, make sure the family is comfortable with the cousin's photo being hosted on a public website. Anyone with the site link may be able to view it.


## Adding the birthday videos later

The video gallery already has 12 cards. For the first test, add your two video files to the `videos` folder and name them:

- `friend-01.mp4`
- `friend-02.mp4`

The first two cards are ready to play those files. The other ten cards remain as placeholders until videos arrive.

When you receive another video:
1. Put it inside the same `videos` folder.
2. Rename it to the next number, e.g. `friend-03.mp4`.
3. Open `index.html` in a text editor and find the `FRIEND_VIDEOS` list near the top of the script.
4. Change that card's `name` and `caption` to the sender's name and a short personal line. Keep the `file` value matching the filename.
5. Re-upload the updated project to GitHub Pages.

You do not need to rebuild the website or change any other code. Keep each filename unique and use `.mp4` for best browser compatibility.

**Animation note:** the bouncing cousin animation is intentionally left untouched for now. Return to it after the video gallery and remaining content are finalised.


## Current test videos

The first two video cards are now populated:
- Card 1: Kartik & Ridhi (`videos/friend-01.mp4`)
- Card 2: Raja & Kishu (`videos/friend-02.mp4`)

For future videos, continue with `friend-03.mp4` through `friend-08.mp4`, then update the matching card's name and caption in the `FRIEND_VIDEOS` list in `index.html`.
