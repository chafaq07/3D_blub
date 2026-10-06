# Take the Captain's Shot

A small interactive browser experiment: a swinging lamp in a dark room, a slingshot, and a bulb you can break and replace.

Built with plain **HTML, CSS and JavaScript**. No frameworks, no build step, no audio files.

## Features

- **Swinging lamp** with simple pendulum physics. Drag it, or hit it with a pebble, and it swings.
- **Light that reveals text.** The page text is only visible inside the cone of light, like reading by a lamp. The cone moves as the lamp swings.
- **Slingshot with aim preview.** Pull the pebble back to see a dotted trajectory, the launch angle and the power.
- **Breakable bulb.** Hit the bulb and it shatters, the room goes dark, and a "Change bulb" button appears.
- **Glass shards** that fall and stay scattered at the bottom of the page.
- **Wall switch** you can click or hit with a pebble to turn the light on and off.
- **Counters** for shots fired and bulbs broken.
- **Sound effects** generated in the browser with the Web Audio API (rope creaks, rubber stretch, snap, glass).
- **Works on desktop and mobile** using pointer events (mouse and touch).

## How to play

1. Drag the pebble back on the slingshot and release to shoot.
2. Hit the **bulb** to break it, the **shade** to make the lamp swing, or the **switch** to toggle the light.
3. After the bulb breaks, press **Change bulb** to install a new one.
4. Drag the lamp to swing it.
5. Use the **sound** button (top right) to mute or unmute.

## Run it locally

No installation is needed.

1. Download or clone this repository.
2. Open `index.html` in any modern browser.

An internet connection is only needed to load the two Google Fonts. Without it, the page falls back to system fonts.

## Deploy with GitHub Pages

1. Push the project to a GitHub repository (the main file should be named `index.html`).
2. Open **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. After a minute, the site will be live at `https://<your-username>.github.io/<repository-name>/`.

## Project structure

```
.
├── index.html   # the whole project: markup, styles and script in one file
└── README.md
```

## Customize

- **Text:** edit the content inside `<div class="txt">` (one `<h1>` and two `<p>` lines). The word inside `<em>` is shown in gold.
- **Hint line:** edit `<div class="hint">`.
- **Page title:** edit the `<title>` tag.
- **Pebble speed:** change the `16` in `pb.vx=dx*16;pb.vy=dy*16` (and the matching `vx=dx*16,vy=dy*16` in the aim preview).
- **Colors:** the main colors are defined at the top of the `<style>` block.

## Tech

- HTML5 Canvas for the lamp, light, slingshot and effects
- CSS for layout and typography
- Vanilla JavaScript for physics and input
- Web Audio API for sound
- Fonts: Bricolage Grotesque and JetBrains Mono (Google Fonts)

## Browser support

Any recent version of Chrome, Edge, Firefox or Safari.

## License

Add a license of your choice (for example MIT) before publishing.
