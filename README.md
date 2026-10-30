<div align="center">

<img src="icon.svg" width="72" alt="Prompter icon">

# Prompter

**A free teleprompter + camera recorder that sits right under your lens.**
Read your script, look at the camera, record in the best quality your device can do. Nothing to install, no account, no uploads.

### [▶ Open the app — prompter-cam-psi.vercel.app](https://prompter-cam-psi.vercel.app)

Works on Windows · Mac · iPhone · Android · any modern browser

</div>

---

## Why

Most teleprompter apps are paid, bloated, or put the text in the middle of the screen so you end up reading *past* the camera. Prompter puts a small black card **right next to your camera** so your eyes stay on the lens, and records you at the same time.

## Features

- **Sits at your camera** – on laptops and portrait phones the card docks at the top, under the webcam. Turn your phone sideways and it moves to whichever edge the front camera is on. Drag it anywhere; double-click the handle to snap it back.
- **Highest-quality recording** – asks for up to 4K, records MP4 (H.264 + AAC) where the browser supports it and falls back to WebM otherwise, with a high bitrate (~12 Mbps at 1080p, up to 60 Mbps at 4K) and studio-style audio (no noise suppression, 48 kHz).
- **Saves locally** – your take is downloaded straight to your device, or sent to Photos / Files with the share sheet on mobile. **Videos never leave your device.** There's no server, no upload, no tracking.
- **Script, font size, speed** – paste your script, then set text size, scroll speed and card size. Everything is remembered for next time.
- **Play · Pause · Restart** – plus tap the text to pause, or drag/scroll it by hand.
- **3-2-1 countdown** – recording starts the scroll automatically.
- **Clean, minimal UI** – black card, white text, one ⚙ settings button to show or hide everything.
- **Pick your camera & mic** – choose external webcams and microphones, or flip front/back on phones.
- **Keeps the screen on** while you record, and works full screen (or as a home-screen app on iPhone).

## Use it

1. Open **[prompter-cam-psi.vercel.app](https://prompter-cam-psi.vercel.app)** and allow camera + microphone.
2. Tap **⚙**, paste your script, set font size and speed.
3. Hit the red **record** button. After a 3-second countdown the text starts scrolling.
4. Hit it again to stop, watch your take, then **Save**.

**Tip:** on iPhone, tap *Share → Add to Home Screen* to run it full screen like a native app.

### Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` | Play / pause |
| `R` | Restart from the top |
| `↑` / `↓` | Faster / slower |
| `F` | Full screen |
| `Esc` | Close settings |

## Recording format by device

| Device | Format |
| --- | --- |
| iPhone / iPad (Safari) | MP4 (H.264) |
| Chrome / Edge on Windows, Mac, Android | MP4 on recent versions, otherwise WebM |
| Firefox | WebM |

Resolution depends on your camera: the app always asks for the highest it offers (up to 4K). The actual resolution and format are shown at the bottom of the settings panel.

## Privacy

Everything runs in your browser. Your script is stored only in your browser's local storage, and your recordings exist only on your device until you save them. Nothing is sent anywhere.

## Run it yourself

It's a single HTML file with no build step and no dependencies.

```bash
git clone https://github.com/codderv006/teleprompter-for-all
cd teleprompter-for-all
npx serve .
```

Camera access requires HTTPS or `localhost`. To host your own copy, deploy the folder to Vercel, Netlify, GitHub Pages or any static host.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/codderv006/teleprompter-for-all)

## Contributing

Issues and pull requests are welcome. If Prompter helped you make a video, a ⭐ on the repo helps other creators find it.

## License

[MIT](LICENSE)
