# Ai-DeskBuddy by ESC LABS

A pocket-sized AI voice assistant with expressive eyes, built on an ESP32-S3-Zero.
It has three modes (AI Assistant, DeskBuddy and Game Clock), switched by voice or by holding the touch pad.

**Live site:** `https://<your-username>.github.io/<repo-name>/`

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The whole website: live OLED simulator, modes, voice commands, wiring, browser installer |
| `images/` | Product photo and wiring diagram |
| `firmware/` | Ready-to-flash firmware (1.3" SH1106 and 0.96" SSD1306), flashed at address `0x0` |
| `manifest-*.json` | Tell the "Connect & install" button which firmware to flash |
| `.nojekyll` | Makes GitHub Pages serve the files as they are |

## Publish on GitHub Pages

1. Create a new **public** repository on GitHub, for example `deskbuddy`.
2. Click **Add file → Upload files** and drag in *everything in this folder*, including the `images` and `firmware` folders. Then click **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: main**, folder **/ (root)**, then click **Save**.
4. After a minute your site is live at `https://<your-username>.github.io/deskbuddy/`.

The "Connect & install" button needs the site to be served over https (GitHub Pages is) and a Chrome or Edge browser on a computer.

## Firmware note

The firmware here is the **public** build: it has no OpenWeather API key built in.
After installing, open the settings page shown on the DeskBuddy screen and enter your city and your own free API key from openweathermap.org.

## Credits

- Built on [xiaozhi-esp32](https://github.com/78/xiaozhi-esp32) (MIT licence)
- 5×7 pixel font from Adafruit GFX (BSD licence)
- Made by [ESC LABS](https://www.esclabs.in)
