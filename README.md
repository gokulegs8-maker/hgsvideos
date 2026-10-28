# HGS VIDEOS website

This is a responsive, single-file website with the exact flow requested:
1. First page says HGS VIDEOS and explains the site.
2. “GO & EXPERIENCE” opens a season selection page.
3. Clicking a season opens a season information page.
4. “Play Season” opens the video in an overlay with Full screen and Minimize controls.

## Add the real season videos
1. Upload each season video to your chosen video host (YouTube Unlisted is a simple option if link-based access is okay).
2. Open `index.html` in a text editor.
3. Find `const seasons = [` in the script near the bottom.
4. Replace `VIDEO_ID_SEASON_1`, etc. with each season video's YouTube ID.
   Example: `https://www.youtube.com/watch?v=AbCdEf12345` -> `AbCdEf12345`
5. Edit each season's `description`, `what`, `subtitle`, and `mood` to match your real season.
6. Save the file.

This starter currently assumes one video per season. If you want several video files within a season, we can change each season page to show a playlist of videos while keeping the seasons page episode-free.

## Publish with GitHub Pages
1. Create a GitHub repository, e.g. `hgs-videos`.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Under build and deployment choose **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
5. Wait for the published URL shown in the Pages settings.

## Important storage and privacy notes
- Do not upload 10+ GB of videos into the GitHub repository. GitHub Pages should host the small HTML website only.
- GitHub Pages does not provide built-in password protection for the site.
- Unlisted YouTube videos are not truly private: anyone with the video link can watch and share them.
- If you want access limited to selected friends, use a video host and authentication setup designed for private content.
