# Password Breaker — Playable on GitHub Pages

A small client-side password-guessing game (like Wordle but for short passwords). It runs entirely in the browser and is ready to be hosted with GitHub Pages.

Features
- Three difficulty levels (easy / medium / hard)
- Feedback per character: green = correct position, yellow = present elsewhere, gray = absent
- Adjustable max attempts
- Local stats stored in localStorage (games, wins, best score)
- Single-file HTML — drop into a repo and enable GitHub Pages

How to deploy
1. Create a new GitHub repository (or use an existing one).
2. Add this `index.html` file to the repository root and push.
3. In the repo Settings → Pages (or Settings → Code and automation → Pages), set the source to the branch you pushed (e.g., `main`) and the root folder `/`.
4. Wait a minute, then open the provided GitHub Pages URL (something like `https://<username>.github.io/<repo>/`) and play.

Notes
- The game is purely client-side; nothing is sent to any server.
- If you want to tweak rules, change the character pools and lengths inside `index.html` (look for `pools` and `genSecret`).
- For debugging, open the browser console — the secret is printed to the console when a new game starts (comment out that line if you prefer).

Enjoy!
