# betterDC

betterDC is a CSS theme for Discord desktop with Vencord. It adds a dark purple gradient or your own wallpaper behind the server list, channel list, and chat. The wallpaper fills the window and the main panels are translucent.

betterDC is an independent project unaffiliated with Discord or Vencord.

## Install on Windows

1. If needed, run the Vencord Windows installer, select your Discord installation, and click **Install**. Reopen Discord. [Vencord download](https://vencord.dev/download/)
2. In Discord, open **User Settings → Appearance** and choose **Dark** or **Midnight**.
3. Download the stylesheet using GitHub's **Download raw file** button. [betterDC.theme.css](betterDC.theme.css)
4. In **User Settings**, find the **Vencord** section and open **Themes → Local Themes → Open Themes Folder**. Copy the downloaded file into that folder.
5. Back in **Local Themes**, click **Load missing Themes** and turn on **betterDC**.

To use QuickCSS, open **Edit QuickCSS** in **Local Themes** and paste the entire stylesheet. Turn on **Enable Custom CSS** in **User Settings → Vencord**.

## Change the wallpaper

Open your installed theme file in Notepad, or edit it in QuickCSS. In the `:root` block at the top, replace `none` with `url("https://i.imgur.com/YOUR_IMAGE.jpg")` and save. Use a direct link to your own image. Vencord allows image hosts such as `i.imgur.com` and `raw.githubusercontent.com`.

| Setting | Default | What it controls |
| --- | --- | --- |
| `--betterdc-wallpaper-image` | `none` | Use `url("...")` for an image or `none` for the gradient. |
| `--betterdc-wallpaper-position` | `center` | Where the image sits as it fills the window. Try `center top` or `25% 50%`. |
| `--betterdc-overlay-opacity` | `0.58` | How much the wallpaper is darkened, from `0` to `1`. |
| `--betterdc-panel-opacity` | `0.56` | How opaque the main panels are, from `0` to `1`. |

Raise either opacity if text is hard to read over a bright image. To use an image from your PC, place it in the Themes folder and use `url("vencord:///themes/wallpaper.jpg")`, with your image's filename.

## Restore Discord's appearance

Turn off **betterDC** in **Local Themes**. If you installed it through QuickCSS, remove the betterDC stylesheet from the editor. If you changed Discord's appearance mode, reselect your previous mode.

## Compatibility

The theme targets Discord desktop with Vencord in dark appearance modes. Discord updates can change the panel selectors. The theme was checked against Vencord's theme-loading source and tested in a Chromium fixture. Live Discord desktop testing was unavailable. [Vencord theme loader](https://github.com/Vendicated/Vencord/blob/ce9355e9a93e369c7295fa162ad563f7f97b1ff7/src/api/Themes.ts)
