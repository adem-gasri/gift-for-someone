# Gift for Faiza 💕

A small interactive birthday gift webpage made with HTML, CSS, and JavaScript.

## Features

- 🔐 PIN-protected opening screen
- 💌 Personalized birthday message
- 📸 Polaroid-style memory photos
- 🎙️ A playable voice note
- 🎵 Two playable songs
- ✨ Animated petals, waves, and page transitions
- 📱 Responsive layout for desktop and mobile

## Project files

```text
gift-for-someone/
├── gift-for-someone.html
├── photo1.jpg
├── photo2.jpg
├── photo3.jpg
├── photo4.jpg
├── voice-note.mp3
├── song.mp3
├── song2.mp3
└── README.md
```

> Keep the image and audio files in the same folder as `gift-for-someone.html` unless you change their paths in the HTML.

## Adding the songs

The page has two song players:

- **A little song** → `song.mp3`
- **Another song** → `song2.mp3`

Put both files next to the HTML file. The second player is already configured to use `song2.mp3`.

If your second file has a different name, for example `love-song.mp3`, change:

```html
<audio id="bg-music-2" src="song2.mp3" preload="metadata"></audio>
```

to:

```html
<audio id="bg-music-2" src="love-song.mp3" preload="metadata"></audio>
```

## Adding photos

Replace the existing photo files with your own images, keeping the same filenames, or change the `src` values in the HTML:

```html
<img class="photo" src="photo1.jpg" alt="Memory">
```

## Run locally

In VS Code, install **Live Server**, then right-click `gift-for-someone.html` and choose **Open with Live Server**.

You can also open the HTML file directly in a browser.

## Update GitHub

After adding or changing files:

```bash
git add -A
git commit -m "Update gift website"
git push
```

If the project is published with GitHub Pages, the website will update automatically after GitHub finishes deploying the new commit.

## Important

Browsers generally block autoplay with sound until the visitor interacts with the page. The songs therefore play when the user presses their play buttons.
