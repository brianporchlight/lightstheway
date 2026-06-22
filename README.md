# Light the Way

Your personal site for writing on mental health — first responders and beyond — and a home for PorchLight. Dark, textured, with a word that glows and changes: *Love lights the way… Grounding lights the way… Mindfulness lights the way…*

This file is your map. Read it top to bottom once; it walks you from "files on my Mac" to "live at LightTheWay.org," and then hands the ongoing work to Cowork.

---

## 1. What's in this folder

```
lighttheway/
├── index.html                  ← the homepage (hero, essays, PorchLight, footer)
├── articles/
│   └── the-drive-home.html     ← a finished sample essay + your reusable template
├── .gitignore                  ← tells Git to ignore Mac clutter (you can ignore this)
└── README.md                   ← you're reading it
```

Everything is plain HTML — no build step, no installing anything to run it. Each page is one self-contained file you can open and read. That's deliberate: it keeps things simple while you learn, and it makes the site effortless to put online.

---

## 2. See it right now

Double-click `index.html`. It opens in your browser and runs — the word will start cycling, the glow will breathe. (When you're online the elegant fonts load automatically; offline you'll see a clean fallback, which is normal.)

---

## 3. Make it yours — the three things you'll change first

You can edit any of these by hand in any text editor, **or** just ask Cowork to do them (section 6). Either way:

- **The glowing words.** Open `index.html`, scroll to the bottom, find the line that starts `const WORDS =`. Add or change the words in that list. Keep them short.
- **The About text.** In `index.html`, find the `ABOUT` section. There's a comment marking the line to rewrite in your own voice.
- **The PorchLight link & your LinkedIn.** Search `index.html` for `href="#"` — those are placeholders. Drop in your real PorchLight and LinkedIn URLs.

**To add a new essay:** copy `articles/the-drive-home.html`, rename it (e.g. `articles/hypervigilance.html`), replace the title and text inside, then add a matching card on the homepage (copy one of the existing `<a class="piece">` blocks). Your Gamma articles go in the same way — paste the writing into a copy of the template.

---

## 4. Put it online (the one-time setup)

Three steps: your files go to **GitHub** (storage + history), **Vercel** turns them into a live site (free), and **GoDaddy** points LightTheWay.org at it. You can do this whole section by hand — no terminal needed — or have Cowork do most of it for you.

### 4a. Get the files onto GitHub
1. Go to **github.com**, sign in (you already have an account from PorchLight), click **+ → New repository**.
2. Name it `lighttheway`, keep it **Public** (free hosting needs this), click **Create repository**.
3. On the new repo page, click **uploading an existing file**, then drag in everything from this folder (`index.html`, the `articles` folder, `.gitignore`, `README.md`). Click **Commit changes**.

That's your repo. Every future change creates a new saved version you can always roll back to.

### 4b. Turn it into a live website with Vercel
1. Go to **vercel.com**, click **Sign up**, and choose **Continue with GitHub** (so they're linked).
2. Click **Add New → Project**, find your `lighttheway` repo, click **Import**, then **Deploy**.
3. About a minute later you'll get a live link like `lighttheway.vercel.app`. Your site is on the internet.

From now on, anything that changes in the GitHub repo auto-publishes here within a minute. You never "upload to a server" again.

### 4c. Point LightTheWay.org at it
1. In Vercel, open your project → **Settings → Domains** → type `lighttheway.org` → **Add**.
2. Vercel will show you **the exact DNS records to enter** (usually one record for the root domain and one for `www`). Copy those exact values — don't guess them, and don't trust values from anywhere else, because they change.
3. In **GoDaddy**: open your domain → **DNS / Manage DNS**, and add the records Vercel gave you.
4. Wait — anywhere from a few minutes to a few hours — and LightTheWay.org will open your site, with the secure padlock added automatically.

> One safety note: enter those DNS records yourself inside your own GoDaddy account. I can talk you through each field, but changing your domain's settings is the kind of thing you should do with your own hands on the controls.

---

## 5. The everyday loop, once it's live

```
   edit a file  →  save to GitHub  →  Vercel republishes  →  live in ~1 min
```

That's the whole rhythm. No re-uploading, no fuss. Write, save, and the world sees it.

---

## 6. Hand it to Cowork

Cowork lives in your **Claude desktop app** on your Mac, in the tab next to Chat and Code. It's the same engine as Claude Code, but you talk to it in plain English and watch it work — no terminal. This site is the perfect first project to learn it on.

**Set it up:**
1. Move this `lighttheway` folder somewhere tidy (e.g. `~/Sites/lighttheway`), not in Downloads.
2. Open the Claude desktop app → **Cowork** tab → point it at this folder.

**Then just talk to it.** Good first things to say:

- *"Walk me through this folder and explain what each file does."* — a guided tour, so you understand what you own.
- *"Change the cycling words to: Love, Grounding, Mindfulness, Breath, Stillness, Hope."*
- *"Here's a new essay I wrote in Gamma — add it as a new article page and put a card for it on the homepage."* (paste the text)
- *"Make the gold a little warmer."* or *"Slow the word changes to every 4 seconds."*
- *"Help me push these changes to my GitHub repo."* — once you've connected it, Cowork handles saving to GitHub, and Vercel republishes on its own.

Cowork shows you its plan and waits for your okay before doing anything, so you stay in the driver's seat the whole time. That's your classroom: change something, watch how it's done, and little by little the mystery disappears.

---

## 7. If you ever feel stuck

Nothing here can break in a way you can't undo — that's the point of GitHub keeping every version. Worst case, you roll back to a version that worked. Start small, change one thing, see it go live, and let the confidence build from there.

Welcome to your own place. Go turn the light on.
