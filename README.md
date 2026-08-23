# The Consilium Retreat — website

A single-file website (`index.html`) for the IEC retreat, ready to host free on GitHub Pages.

## Host it free on GitHub Pages (~5 minutes)

1. Go to [github.com/new](https://github.com/new) and create a repository. Name it anything, e.g. `consilium-retreat`. Set it to **Public** (required for free Pages hosting).
2. On the new repo's page, click **"uploading an existing file"**, drag in `index.html` (and this README if you like), and click **Commit changes**.
3. Go to the repo's **Settings → Pages** (left sidebar).
4. Under "Build and deployment," set **Source** to "Deploy from a branch," choose the **main** branch and **/ (root)** folder, and click **Save**.
5. Wait 1–2 minutes, then refresh the Pages settings page. Your live URL appears at the top, like:
   `https://YOUR-USERNAME.github.io/consilium-retreat/`

That's it. Any time you edit and re-upload `index.html`, the site updates automatically.

**Want a custom domain later** (e.g. consiliumretreat.com)? Buy the domain anywhere (~$10/yr), then add it in Settings → Pages → Custom domain and point the domain's DNS at GitHub per the instructions shown there. The hosting itself stays free.

## Connect your Google Form (~3 minutes)

The application form is a Google Form embedded in the page, so all responses land in your Google account (and can feed a Google Sheet automatically).

1. Go to [forms.google.com](https://forms.google.com) and create a form. Suggested fields:
   - Full name (short answer, required)
   - Email (short answer, required — or turn on "Collect email addresses" in the form's Settings)
   - Practice / company (short answer)
   - Years as an IEC (multiple choice: Just getting started / 1–3 years / 4–9 years / 10+ years)
   - Room preference (multiple choice: Shared room, $1,599 / Private room, $1,999)
   - If shared: anyone you'd like to room with? (short answer)
   - Interested in the Bogotá sightseeing add-on? (Yes / Maybe / No)
   - Anything you'd like us to know? (paragraph)
2. Click **Send** (top right) → the **`< >`** embed tab → copy the URL inside `src="..."`. It looks like:
   `https://docs.google.com/forms/d/e/1FAIpQLSe.../viewform?embedded=true`
3. Done — the live form ID is already wired into `index.html`.

Tip: in the form editor, open **Responses → Link to Sheets** to get every application in a spreadsheet, and turn on email notifications under Responses → ⋮ → "Get email notifications for new responses."

If the embedded form looks cramped, you can adjust its height in `index.html` — search for `height:1050px`.

## Photos

The `images/` folder is already prepared — upload it to your repo along with `index.html` (drag the whole folder into GitHub's upload page). Current photo assignments:

| Filename | What it shows | Where it appears |
|---|---|---|
| `images/hero.jpg` | Golden-hour aerial of the cabins | Hero |
| `images/property-1.jpg` | Blue-sky coffee vista | Property gallery |
| `images/property-2.jpg` | Bright cabin room | Property gallery |
| `images/property-3.jpg` | Deck view of the mountains | Property gallery |
| `images/property-4.jpg` | Stilted cabin with deck | Property gallery |
| `images/property-5.jpg` | Plated meals | Property gallery |
| `images/property-6.jpg` | Stone path through the coffee | Property gallery |
| `images/room-shared-1.jpg` … `-9.jpg` | Shared room, deck view, bathroom set, net | Shared room card, scrollable |
| `images/room-private-1.jpg` … `-10.jpg` | Private room, deck view, bathroom set, net | Private room card, scrollable |
| `images/excursion-coffee.jpg` | Coffee tasting group | Coffee tasting card |
| `images/excursion-fruit.jpg` | Fresh fruit spread | Fruit tour card |
| `images/excursion-hiking.jpg` | Forest bridge hike | Hiking card |
| `images/excursion-biking.jpg` | Mountain biker on the outcrop | Mountain biking card |
| `images/excursion-dancing.jpg` | Latin dancing | Dancing card |
| `images/event-1.jpg` … `-3.jpg` | Note-taking, workshop & event space | Program section strip |
| `images/excursion-horseback.jpg` | Horseback riding | Horseback card |
| `images/org-caitlin.jpg`, `images/org-quyen.jpg` | Organizer headshots | Organizers section |

To swap any photo, just replace the file with a new one using the same name. Landscape images around 1600px wide work best.

## Things marked for you to edit

Search `index.html` for `EDIT:` comments:
- The **Google Form ID** — see above.
- The **photos** — see above.
- The **Organizers section** — real bios for Quyen and Cornell, Caitlin's last name, and photos if you'd like (swap each avatar `div` for an `<img>`).
- The **day-by-day schedule** — session titles, once the program is locked.

## Renaming the retreat

If "Consilium" changes, find-and-replace `Consilium` in `index.html` — it appears in the page title, header, and apply section.
