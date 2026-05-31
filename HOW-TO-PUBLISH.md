# How to publish your privacy + terms pages

≈ 5 minutes, all done in a web browser. No command line needed.

The two files in this folder (`privacy.html`, `terms.html`) are already named exactly right. After you upload them, they will live at:

- `https://connection-cmd.github.io/diplomats-handbook/privacy.html`
- `https://connection-cmd.github.io/diplomats-handbook/terms.html`

The app's paywall already points at those URLs.

---

## 0. Fill in the three placeholders first (≈ 2 minutes)

Open both files in this folder in a text editor (Notepad, VS Code, anything). Use **Find and Replace** to fill in these three placeholders **in both files**:

| Placeholder | What to put |
|---|---|
| `[Publisher name]` | Your legal entity / sole-trader name, e.g. **Abdulla [Last name]**, or a business name if you have one set up |
| `[contact email]` | A real email you check (can be a Gmail), e.g. `support@yourdomain.com` or `youraddress@gmail.com` |
| `[Jurisdiction]` | Only in `terms.html` — the country/emirate whose courts govern disputes, e.g. **Dubai, United Arab Emirates**, or wherever you legally reside / are registered |

Save the files.

> If you'd rather have me suggest defaults, send me your name + an email + your country and I'll fill them in for you.

---

## 1. Create a free GitHub account (if you haven't already)

You're logging in as **`connection-cmd`** — the username already baked into the app. Skip to step 2 if you already use this account.

Otherwise: go to **github.com**, click **Sign up**, use the username `connection-cmd` and any email/password.

---

## 2. Create the repository

1. Once signed in, click the **+** icon top-right → **New repository**.
2. **Repository name:** `diplomats-handbook` (exactly, lowercase, with the hyphen).
3. **Description:** *optional*, e.g. "Privacy policy and terms for The Diplomat's Handbook app."
4. **Public** (must be public for free GitHub Pages).
5. **Do not** tick "Add a README" / "Add .gitignore" / "Choose a license" — leave the repo empty.
6. Click **Create repository**.

---

## 3. Upload the two files

On the empty repo page, GitHub shows a line that says:

> "uploading an existing file"

(it's a hyperlink — about halfway down).

1. Click that link.
2. Drag both files from this folder (`Co-Work\store-launch\github-pages\privacy.html` and `terms.html`) onto the upload area. Or use the **choose your files** button.
3. Scroll down. **Commit message:** "Initial publish."
4. Make sure **"Commit directly to the `main` branch"** is selected.
5. Click **Commit changes**.

You should now see both files in the repo.

---

## 4. Turn on GitHub Pages

1. In the repo, click **Settings** (top tabs).
2. In the left sidebar, click **Pages**.
3. Under **Source**, choose **Deploy from a branch**.
4. Branch: **`main`**. Folder: **`/ (root)`**. Click **Save**.
5. The page will reload and show a banner that says something like *"Your site is live at https://connection-cmd.github.io/diplomats-handbook/"*. (It can take 1–2 minutes the first time.)

---

## 5. Verify

In a new browser tab, open each URL and confirm the page renders nicely (cream background, serif fonts):

- https://connection-cmd.github.io/diplomats-handbook/privacy.html
- https://connection-cmd.github.io/diplomats-handbook/terms.html

If either gives a 404, wait another minute (GitHub is still building) and refresh.

---

## 6. You're done

The app already points at these URLs, so the **Terms** and **Privacy** buttons on the paywall will now open them.

Tell me when they're live and I'll also paste the privacy URL into the Play Console listing in the next step.

---

## Updating later

To make changes to either document:

1. Open the file in the GitHub repo (just click it on the repo page).
2. Click the pencil icon (top-right of the file view) to edit.
3. Edit. Scroll down. **Commit changes.**

The live page updates within seconds.

If you'd rather I do edits for you, send me the change and I'll regenerate the file — you just need to re-upload it (drag-drop onto the repo overwrites the existing copy).

---

## Why we didn't push from this machine

The GitHub CLI (`gh`) isn't installed on this machine, so I can't authenticate as you or push on your behalf. Installing it + logging you in would take longer than the 5-minute web upload above, so the manual path wins. If you ever want me to do these via CLI in future, install **GitHub CLI** from `cli.github.com` and run `gh auth login` once.
