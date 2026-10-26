# Project Liftoff: Neo-Colombo 2027

A live software project-management simulation for the NIBM industry visit.

## Files
- `index.html`: the whole game (crews, Game Master console, optional second screen)
- `img/`: scene art (hero + ch0 to ch7)

## 1. Create the live database (Firebase, free)
1. Go to https://console.firebase.google.com, choose **Add project**, name it `project-liftoff`, turn off Analytics.
2. In the left menu: **Build > Realtime Database > Create database**.
3. Location: **Singapore (asia-southeast1)**. Security rules: **Start in test mode**.
4. Copy the database URL shown at the top (it ends in `firebasedatabase.app` or `firebaseio.com`).
Test mode stays open for 30 days. Only game choices are stored. Delete the project after the event.

## 2. Publish on GitHub Pages
1. On GitHub: **New repository**, name `project-liftoff`, **Public**, create.
2. **Add file > Upload files**: drag in `index.html`, `README.md` and the whole `img` folder. Commit.
3. **Settings > Pages**: Source **Deploy from a branch**, branch **main**, folder **/ (root)**, Save.
4. After about a minute your game is at `https://<your-username>.github.io/project-liftoff/`.

## 3. Connect the console
1. Open `https://<your-username>.github.io/project-liftoff/?host=1`
2. **Setup and links**: paste the Firebase URL, set a session code (e.g. `dryrun`), choose 6 or 8 crews, **Save and connect**. The pill turns green: **Live**.
3. **Show crew QR codes**: each code carries the session and database, so crews need nothing else.
Keep the console link to yourself. Crew links have no controls.

## Game-day flow (per mission)
Briefing (crews read, cards locked) > Open voting (timer) > Close voting > your story > Reveal > Next mission.
Crews can only lock in. Only the console moves everyone forward.
Use a fresh session code for the real run (e.g. `nibm`).
