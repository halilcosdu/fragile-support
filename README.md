# Fragile - Privacy & Support

The public site for **Fragile**, a packing puzzle for iPhone and iPad published by Halil Cosdu.
It doubles as the App Store privacy policy and support page, and shows the game itself with the
same screenshots that are on the store listing.

| Page | URL |
|---|---|
| English | https://halilcosdu.github.io/fragile-support/ |
| Türkçe | https://halilcosdu.github.io/fragile-support/tr.html |

App Store Connect fields, per localization:

| Field | English | Türkçe |
|---|---|---|
| Privacy Policy URL | `/fragile-support/` | `/fragile-support/tr.html` |
| Support URL | `/fragile-support/#support` | `/fragile-support/tr.html#support` |
| Marketing URL | `/fragile-support/` | `/fragile-support/tr.html` |

## What is here

```
index.html      English page
tr.html         Turkish page - same structure, its own screenshots
site.css        one stylesheet for both
wordmark.png    the game's wordmark, rendered from the app's own font and gradient
icon.png        the App Store icon at 256px, used as the favicon
media/          web-sized WebP copies of the store screenshots (en/ and tr/) plus the hero backdrop
```

Two hand-written HTML files and one stylesheet: no build step, no framework, no JavaScript. The
language switch is a plain link, so it works with scripting disabled, and each page carries the
correct `lang` and `hreflang`.

Nothing is loaded from a third party - no web fonts, no scripts, no analytics, no cookies - which is
the same standard the app is held to: Fragile collects no data, has no account, shows no ads and
makes no network requests at all.

The images come from the game: `media/` is generated from the App Store screenshot set by
`Tools/support_site_media.py` in the game project, and the wordmark by `Tools/launch_wordmark.py`.
