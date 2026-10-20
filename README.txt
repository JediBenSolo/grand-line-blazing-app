Grand Line Blazing - iPhone app kit

1. Make a free GitHub account, then a new PUBLIC repository (free GitHub Pages, which delivers the
   over-the-air updates, only works on public repositories).
2. In the repository: Settings > Pages > Build and deployment > Source: "GitHub Actions".
3. Click "uploading an existing file" and drag in EVERYTHING in this folder, including the .github folder
   (if it gets left out: use "Add file > Create new file", type .github/workflows/build-ios.yml and paste
   that file's contents).
4. Open the Actions tab. The "Build iPhone app" run starts by itself (or press "Run workflow"). It takes ~10 minutes.
5. When it shows a green tick, open the run and download GrandLineBlazing-ipa (a zip holding GrandLineBlazing.ipa).
6. On your PC install Sideloadly (sideloadly.io) and iTunes (from apple.com, not the Microsoft Store), plug in the
   iPhone, drag the .ipa into Sideloadly, enter your Apple ID and press Start.
7. On the iPhone: Settings > General > VPN & Device Management > trust your Apple ID.
   (iOS 16+: also Settings > Privacy & Security > Developer Mode > On, then restart.)
With a free Apple ID the app must be re-signed every 7 days: just run Sideloadly again (your save is kept).

UPDATES OVER THE AIR
When the game changes you get new www.zip.001, .002, ... and version.json. Upload just those files to the repository
(replace the old ones). The update goes live in a few minutes; the app downloads it the next time it opens and
installs it the time after that. No Sideloadly needed for game updates.
