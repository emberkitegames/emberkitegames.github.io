# emberkitegames.github.io

The website for Emberkite Games. One site for every game: home page, one page per
game, one privacy policy, one support page, and one app-ads.txt file.

## Links to paste into Play Console (for every game)

| Play Console field | Link |
|---|---|
| Privacy policy | https://emberkitegames.github.io/privacy-policy.html |
| Website | https://emberkitegames.github.io |
| Email | emberkitegames@gmail.com |

## Put it online (one time, about 15 minutes, no coding)

1. Create the Gmail `emberkitegames@gmail.com` (if it is taken, see "Changing the email" below).
2. Go to github.com and sign up with that Gmail. Username: **emberkitegames** (exactly).
3. Click **+** (top right) → **New repository**.
   - Repository name: **emberkitegames.github.io** (exactly this)
   - Public
   - Click **Create repository**.
4. On the next page click **uploading an existing file**.
5. Unzip this folder on your laptop. Open it, select **everything inside** (the `assets` and
   `games` folders and all the files), and drag it into the GitHub page.
6. Scroll down, click **Commit changes**.
7. Go to **Settings → Pages**. Under "Branch" choose **main** and **/ (root)**, click **Save**.
8. Wait 1–2 minutes, then open https://emberkitegames.github.io

## Changing the pictures

The pictures of the game live in `assets/img/games/escape-from-war-zone/`.
To replace one, upload a new file with **exactly the same name**:

| File | Size | Used on |
|---|---|---|
| `icon.png` | 256×256 | home card, game page |
| `feature.jpg` | 1024×500 | home card |
| `banner.jpg` | 1600×780 | top of the game page |
| `screen-1.jpg` … `screen-4.jpg` | 1280×672 | screenshots row |
| `../../og-image.jpg` | 1200×630 | the preview when someone shares a link |

When Claude Code finishes Step 6 (new icon and store images), swap them in.

## Adding a new game

1. Put its pictures in `assets/img/games/<game-name>/` (icon.png 256×256, feature.jpg 1024×500, screenshots).
2. Copy `games/escape-from-war-zone.html` to `games/<game-name>.html` and change the text and pictures.
3. In `index.html`, copy the block between `<!-- GAME START -->` and `<!-- GAME END -->`,
   paste it underneath, and edit it.
4. In `privacy-policy.html`, add one row to the table of games, and change "Last updated".
5. Upload the changed files to GitHub the same way (Add file → Upload files).

The privacy policy link and website link never change, so older games keep working.

## When your game goes live on Google Play

1. **Play button:** in `games/escape-from-war-zone.html`, find the comment
   `PLAY STORE BUTTON` and follow it (replace the "Testing now" line with the
   "Get it on Google Play" button). Do the same in `index.html` if you like:
   change the "Testing now" label to "Out now on Google Play".
2. **Status:** in the game page's details box, change `Closed testing` to `Available`.
3. **app-ads.txt:** see below.
4. Upload the changed files to GitHub.

## app-ads.txt

AdMob gives you one line after you link your published game. Open `app-ads.txt`,
follow the instructions inside, and upload it again. One line covers all your games.

## Changing the email

The email `emberkitegames@gmail.com` appears in every page. If you use a different
one, open the folder in VS Code, press Ctrl+Shift+H (Replace in files), and replace
it everywhere.

## Credits

Fonts: Baloo 2 (Ek Type) and Mukta (Ek Type), SIL Open Font License 1.1 (see `assets/fonts`).
