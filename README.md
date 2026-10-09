# AgentSearch @ ICLR 2027

Website for **AgentSearch: Constructing and Evaluating Agentic Solutions in Open Ecosystems**, the second AgentSearch workshop (proposed for ICLR 2027).
Previous edition: [AgentSearch @ SIGIR 2026](https://agent-search.github.io/agentsearch-sigir26/).

Planned URL: https://agent-search.github.io/agentsearch-iclr27/

## Structure

Plain HTML/CSS/JS, no build step. Uses the SIGIR 2026 site's design: `style.css` and `main.js` are copied from that repo, and ICLR-specific rules sit in the "ICLR 2027 additions" block at the end of `style.css`.

```
index.html              single-page site
assets/css/style.css    styles (SIGIR 2026 + additions at the end)
assets/js/main.js       mobile menu, scrollspy, back-to-top
assets/img/             logo, organizers/, speakers/
```

Preview locally with `python3 -m http.server 8000`, then open http://localhost:8000.

## Deploy

GitHub repo → Settings → Pages → deploy from `main` branch, root folder.

## Common edits

- **Speaker / organizer photos**: add the image to `assets/img/speakers/` or `assets/img/organizers/` and replace `assets/img/placeholder.svg` in that person's `<img src>`.
- **Hero photo**: add `assets/img/hero-background.jpg` (e.g. San Francisco) and delete the gradient `.hero-background` rule at the end of `style.css`.
- **After the ICLR decision (Nov 29, 2026)**: update the "Proposal under review" note in the hero and the footer.
- **Dates**: the "Important Dates" box in the Call for Papers section.
