# Plenty brand assets

Everything here except the two masters is rendered by `bin/brand-assets` from those masters, in the
site's fonts (`assets/fonts`) and colours (`assets/css/site.css`). Edit a master or the script, then
render again on the GPU:

```sh
gpu-lock bin/brand-assets                         # everything
gpu-lock bin/brand-assets --only banners          # or marks, favicons, wordmarks
gpu-lock bin/brand-assets --overlay /tmp/overlay  # also draws each banner's safe area, to check by eye
```

The banner step fails if any text or logo ink leaves the platform's safe area, or the headline loses
its two lines.

"Light" means for light backgrounds: ink `#17150f` and red `#c7361c` (on paper `#f4f0e6`). "Dark" means
for dark backgrounds: ink `#f2ede2` and red `#ff6a48` (on `#121110`).

## Masters

| File | What it is |
| --- | --- |
| `plenty-mark.svg` | The "p." mark on its square canvas, optically centred (commit 74b3248): its visual weight, not its bounding box, sits in the middle, and it stays inside a circle inscribed in the canvas, so round and square crops both work. Follows the system's light or dark mode. |
| `plenty-wordmark.svg` | The outlined "plenty." wordmark the site's header uses. Follows the system's light or dark mode. |

## The mark

Each folder has `plenty-mark-light.svg` and `plenty-mark-dark.svg`, plus PNGs of each at 16, 32, 48, 64,
128, 180, 192, 256, 512 and 1024 pixels (`plenty-mark-light-512.png`).

| Folder | What it is | Use it for |
| --- | --- | --- |
| `mark/square/` | The mark on a full, opaque square of the brand background. | Profile pictures on services that crop for you: GitHub organisation avatar, X, LinkedIn company logo, Mastodon, YouTube, Facebook. Upload the 1024 PNG; each service applies its own circle or rounded square, and the mark stays centred in either. |
| `mark/circle/` | The mark on a circle of the brand background, with transparent corners. | Places that show the image as is and want it round: slides, documents, email signatures, chat apps without their own crop. |
| `mark/transparent/` | The mark alone. | Placing on your own background. Use light on light backgrounds, dark on dark. |

## Favicons

| File | Use |
| --- | --- |
| `favicon/favicon.svg` | The site's icon: the mark on a rounded square, light or dark with the system. |
| `favicon/favicon.ico` | 16, 32 and 48 pixel icon for browsers and tools that don't read SVG. |
| `favicon/favicon-192.png`, `favicon-512.png` | PNG icons (rounded square, light) for browsers and web app manifests. |
| `favicon/apple-touch-icon.png` | 180 pixel, opaque square for iOS home screens, which round the corners themselves. |

## The wordmark

| File | Use |
| --- | --- |
| `wordmark/plenty-wordmark-light.svg`, `-dark.svg` | The wordmark with fixed colours, transparent. |
| `wordmark/plenty-wordmark-light-1024.png`, `-2048.png` (and `dark`) | The wordmark, transparent, 1024 or 2048 pixels wide. |
| `wordmark/plenty-wordmark-light-background-1024.png`, `-2048.png` (and `dark`) | The same on the brand background, with clear space of half its height on every side. |

## Banners

Each keeps its text and logo in the platform's safe area, listed with its size. They use the light
palette, the site's hero lines, and the wordmark.

| File | Size | Use, and what the safe area keeps clear of |
| --- | --- | --- |
| `banners/og-default.png` | 1200x630 | plenty.is link previews (`og:image`, `twitter:image`). Keeps 72px clear left and right and 40px top and bottom. |
| `banners/og-default@2x.png` | 2400x1260 | The same at 2x, for anywhere that takes a sharper preview. |
| `banners/linkedin-company-cover.png` | 4200x700 | LinkedIn company page cover, the size LinkedIn asks for. |
| `banners/linkedin-page-banner.png` | 1128x191 | LinkedIn company page banner at its shown size. Clear of the logo, which overlaps the bottom left on phones. |
| `banners/linkedin-profile-banner.png` | 1584x396 | LinkedIn personal profile background. Clear of the profile picture on the left. |
| `banners/x-header.png` | 1500x500 | X header. Clear of the avatar at the bottom left and of the top and bottom X crops on some screens. |
| `banners/mastodon-header.png` | 1500x500 | Mastodon header. Clear of the avatar at the bottom left. |
| `banners/facebook-cover.png` | 851x315 | Facebook page cover. Inside the middle that phones show. |
| `banners/youtube-channel-banner.png` | 2560x1440 | YouTube channel banner. Inside the middle 1546x423 that phones, computers and TVs all show. |
