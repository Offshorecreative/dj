# Offshore Creative Music

Source export of the [published site](https://offshore-creative-music-bali.distinctoatcake4.chatgpt.site/) from revision `294b563a7a04f4cc8aabb6c404fb79ff838e5ac9`.

## Run locally

Extract the entire ZIP. Open a terminal in the folder containing this README and run the following with Python 3 installed.

```sh
python3 -m http.server 8000 --bind 127.0.0.1 --directory dist
```

On Windows, use `py -3` in place of `python3`. Open **http://127.0.0.1:8000/**. Stop the server with Ctrl+C. The site runs directly in the browser. Dependency installation and compilation are unnecessary.

## Edit the site

- Edit `dist/index.html` for page copy, portfolio entries, gallery images, accessible labels and form fields.
- Edit `dist/style.css` for typography, spacing, layout, responsive breakpoints and interactive states.
- Edit `dist/app.js` for menus, playback, gallery navigation and the inquiry form. Submitting the form opens WhatsApp with the visitor’s message for review and sending.
- `dist/assets/` holds the original site assets, including images, logos and fonts. The MP4s are in `dist/assets/videos/`. When changing a clip, update each reference used by its preview and player, including any poster image.
- `dist/gsap.min.js` is the bundled third-party animation library. The application code is editable directly in the three files above.

## Deploy

Use a static host and publish the **contents of dist/** with `index.html` at the web root. For Git-based hosting, select `dist` as the publish directory and leave the build command empty. Copy the entire asset tree with its original case and filenames. Serve over HTTPS with support for MP4 byte-range requests for seeking. The original ChatGPT Sites manifest in `.openai/hosting.json` identifies the existing project. Other static hosts can ignore it.

## Media and external services

This export serves copies of the following original videos from local paths. The files keep the original encoding and sound. Existing YouTube embeds, outbound links, and WhatsApp messaging require internet access.

| Bundled file | Original source |
| --- | --- |
| assets/videos/Vault Multicam Preview.mp4 | https://raw.githubusercontent.com/Offshorecreative/Multicam-livestreaming/main/Vault%20Multicam%20Preview.mp4 |
| assets/videos/1212121212121212112.mp4 | https://raw.githubusercontent.com/Offshorecreative/Video-creation/main/1212121212121212112.mp4 |
| assets/videos/hero7878787874764.mp4 | https://raw.githubusercontent.com/Offshorecreative/hero/main/hero7878787874764.mp4 |
| assets/videos/BADESSONE-INNO-01.mp4 | https://raw.githubusercontent.com/Offshorecreative/reels/main/BADESSONE-INNO-01.mp4 |
| assets/videos/King-Combs-mesa.mp4 | https://raw.githubusercontent.com/Offshorecreative/reels/main/King-Combs-mesa.mp4 |
| assets/videos/RED-RUBY-9282828.mp4 | https://raw.githubusercontent.com/Offshorecreative/reels/main/RED-RUBY-9282828.mp4 |
| assets/videos/They-call-me-shallipopi!.mp4 | https://raw.githubusercontent.com/Offshorecreative/reels/main/They-call-me-shallipopi!.mp4 |
| assets/videos/midnight838383838.mp4 | https://raw.githubusercontent.com/Offshorecreative/reels/main/midnight838383838.mp4 |
