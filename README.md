# Portfolio website from 30 minutes of prompts (template)

This is the portfolio site I built from scratch with Claude Code in a timed
30-minute speedrun. I didn't type any code by hand, only prompts.

- 🎬 **Video:** _link coming soon_
- 🌐 **Live demo (this exact code):** https://kriggithub.github.io/YT_Portfolio_Website_Template/
- 🧑‍💻 **My current portfolio (it has changed since the video):** https://kriggithub.github.io

> **Frozen at the end of the video.** This repo matches what you saw when the
> timer hit 30:00 (source commit `72db7ff` of the original repo). It isn't
> maintained, so fork it and make it yours.

## What's in it

Plain HTML, CSS and JavaScript: no framework, no build step, nothing to
install. It has three pages (Home, Academic, YouTube), a 404 page, a live
central-limit-theorem simulation, a cursor trail, a ⌘K command palette,
count-up stats and a skills marquee.

## Make it your own

1. Click **Use this template** → **Create a new repository** (make it public).
2. Change the content. The easy way is the way I built it: open the repo in
   Claude Code and paste something like this:

   > Replace Kurt's details everywhere in this site with mine. Name: ___. What I
   > do: ___. Links: GitHub ___, LinkedIn ___, YouTube ___, email ___. Replace
   > the Academic page with ___ (or turn it into a Projects page). Keep the
   > design. If the repo isn't named `YT_Portfolio_Website_Template`, also fix
   > the paths in `404.html`.

   If you'd rather do it by hand:

   | What | Where |
   |---|---|
   | name, typing words, social links, YouTube videos | `js/config.js` |
   | hero text, skills marquee, the two cards | `index.html` |
   | research, R packages, publications, CV button | `academic.html` |
   | channel name and handle | `youtube.html` |
   | page titles, meta tags, footer, `kurt.dev` logo | top and bottom of every `.html` file |
   | colors and fonts | variables at the top of `css/style.css` |
   | 404 page links | `404.html` uses `/<repo-name>/...` paths, so change them to your repo's name (or to `/` if your repo is `<username>.github.io`) |

3. **Put it online (free):** go to your repo → **Settings** → **Pages** →
   *Deploy from a branch* → `main` / `(root)` → **Save**. After about a
   minute it's live at `https://<username>.github.io/<repo-name>/`. Name the
   repo `<username>.github.io` if you want it at the root URL.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## License

MIT. Use it for anything. Credit is appreciated but not required.
