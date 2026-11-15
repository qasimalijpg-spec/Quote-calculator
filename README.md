# Quote Calculator

A simple quote calculator for a clothing manufacturing business (T-shirts, hoodies, trousers, suits).
All prices are in PKR, with an optional USD price for overseas clients.

It works on a computer and on iPhone (Safari), and you can add it to your iPhone home screen like an app.
It is free: no app store, no server and no monthly cost.

## What is in this folder

| File | What it does |
|------|--------------|
| `index.html` | The whole app (the screens, the maths and the design) |
| `manifest.json` | Tells the phone the app's name and icon |
| `sw.js` | Lets the app open even with no internet |
| `icons/` | The app icon |

## Put it online for free (GitHub Pages)

1. Go to your repository on github.com and sign in.
2. Make sure the app files are on the **main** branch (merge the pull request if they are on another branch).
3. Click **Settings** (top of the repository page), then **Pages** in the left menu.
4. Under **Build and deployment** → **Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose **main** and **/ (root)**, then click **Save**.
6. Wait 1–2 minutes and refresh the page. A link appears at the top, like
   `https://YOUR-USERNAME.github.io/Quote-calculator/`. That is your app.

> GitHub Pages is free for **public** repositories. With a public repository, anyone with the link can see the
> app's code and default prices, but **not** your saved quotes or changed prices: those stay only on your device.

## Add it to your iPhone home screen

1. Open the link in **Safari** (not Chrome or Instagram's browser).
2. Tap the **Share** button (the square with an arrow pointing up).
3. Scroll down and tap **Add to Home Screen**.
4. Tap **Add**. The "Quotes" icon now appears on your home screen.

Always open the app from this icon. The home-screen app keeps its own copy of your prices and saved quotes,
separate from Safari.

## Keep your data safe

Your prices and saved quotes are stored **only on the device you use**. They do not sync between phone and computer.
Go to **Settings → Backup** now and then to save a backup file. Use **Restore** to load it on another device.

## How the price is worked out

- **Fabric** = fabric used (kg) × fabric price per kg
- **Cost per piece** = fabric + cutting + stitching + pressing/packing + ticked extras + ticked trims + shipping + (one-off costs ÷ quantity)
- **Shipping** = shipping weight per piece × shipping price per kg (the weight starts as the fabric weight)
- **Quote per piece** = cost per piece + profit % of the cost (for example, cost 1,000 + 25% = 1,250)
- **USD** = PKR amount ÷ dollar rate
