# Tractor Register India — Site Files

This is a multi-page static website: a homepage plus four sub-folders
(`tractors/`, `implements/`, `articles/`, `legal/`), all linked together
with relative paths. Because it's more than one file, the upload steps
are slightly different from uploading a single `index.html`.

## What's in this folder

```
tractor-register-india/
├── index.html          ← homepage (must stay at the root)
├── style.css            ← shared stylesheet (must stay at the root)
├── tractors/            ← brand pages + model spec pages
├── implements/           ← implement detail pages
├── articles/             ← buying guide articles
└── legal/                ← About, Contact, Privacy, Disclaimer
```

Every link inside these pages is relative (e.g. `../style.css`,
`tractors/mahindra.html`), so the **folder structure must be preserved
exactly** when you upload — don't flatten everything into one folder,
and don't rename the sub-folders.

## Option A — Upload via GitHub's website (no extra tools needed)

GitHub's drag-and-drop uploader supports folders in most modern
browsers (Chrome, Edge, Firefox). This is the simplest path:

1. Go to your repository on github.com (the same one you created
   before — e.g. `github.com/yourusername/tractor-register`).
2. Click **Add file** → **Upload files**.
3. **Unzip** `tractor-register-india.zip` on your computer first, so
   you have a normal folder, not a zip.
4. Open that unzipped folder. Select **all of its contents** —
   `index.html`, `style.css`, and the four sub-folders
   (`tractors`, `implements`, `articles`, `legal`) — and **drag all of
   them together** into the GitHub upload area in your browser.
   - Important: drag the *contents* of the folder, not the folder
     itself. If you drag the outer `tractor-register-india` folder,
     everything will end up nested one level too deep
     (`tractor-register-india/index.html` instead of `index.html`),
     and the site won't load correctly at your `github.io` URL.
5. Wait for the upload list to populate — you should see `index.html`,
   `style.css`, and four folder entries listed.
6. Scroll down, write a short commit message (e.g. "Add full site"),
   and click **Commit changes**.
7. If you already have an old `index.html` in the repo from the single
   page version, GitHub will ask if you want to replace it — confirm
   yes.

## Option B — If your browser won't let you drag a folder

Some browsers only accept individual files via drag-and-drop, not
folders. If step 4 above doesn't work:

1. Upload `index.html` and `style.css` at the root first (Add file →
   Upload files → drag just those two).
2. Commit.
3. Click **Add file** → **Upload files** again.
4. Open the `tractors` folder on your computer and drag its *files*
   (not the folder) into the GitHub upload box. GitHub will ask you to
   type the folder name — type `tractors` and it will create that
   folder automatically and place the files inside it.
5. Repeat step 4 for `implements`, `articles`, and `legal`.

This is slower but works in any browser.

## After uploading: confirm it's live

1. Go to **Settings → Pages** in your repo (refer back to your original
   setup steps if you need to re-enable this).
2. Your published URL will be something like
   `https://yourusername.github.io/tractor-register/`.
3. Visit that URL and click through a few links — Home → Tractors →
   Mahindra → Mahindra 575 DI — to confirm everything resolves. If a
   page 404s, the most common cause is a folder that didn't upload, or
   files that landed one level too deep (see the warning in step 4 of
   Option A).

## Monthly updates going forward

Since this site is meant to refresh monthly: the easiest way to update
content is to come back to this chat (or a new one), tell me what's
changed (new model, updated price, new article), and I'll edit the
relevant file(s) and hand you back just the changed file — you can
then re-upload that single file via **Add file → Upload files**,
which will overwrite the existing version in the same folder.
