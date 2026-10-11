# Wedding Bar Planner

An interactive calculator for couples buying their own reception alcohol. Set the guest count, the light / moderate / heavy drinker mix, bar hours, pour sizes, and the split between wine, beer, and spirit drinks. The page returns:

- a liquor shopping list (wine, beer, spirits, core modifiers) with bottle sizes and spare volume after rounding up
- a cocktail menu built from those bottles, plus the drinks that are one or two bottles away and which add-on bottles unlock the most drinks
- mixer, garnish, and ice quantities in a collapsed section for the bar team

Everything runs in the browser. Settings are saved in that browser only (localStorage). Nothing is sent anywhere.

## Run locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

**GitHub Pages:** push this folder to a repository, then in Settings → Pages choose "Deploy from a branch", branch `main`, folder `/ (root)`. The site publishes at `https://<user>.github.io/<repo>/`.

**Personal site:** copy `index.html` into any static path (for example `/tools/wedding-bar/index.html`). There is no build step.

## Method

Pour sizes follow NIAAA standard-drink references (750ml = 25.4 oz; 1.75L = 59.2 oz). Consumption defaults sit inside the 0.75 to 1.0 drinks per guest per hour range that wedding planning guides publish for lighter crowds. All defaults are adjustable on the page, and the Assumptions section lists them.
