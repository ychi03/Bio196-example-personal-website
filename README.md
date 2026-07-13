# BIO196 Personal Website Template

This repository is the starter template for the BIO196 personal website assignment.

You will use this template to practice a real GitHub workflow:

- fork a course template
- customize your own copy
- publish a website with GitHub Pages
- submit your repository link and website link
- later, contribute your links back to the course submissions repository

## What you will create

By the end of the assignment, you should have:

- your own GitHub repository named `bio196-personal-website`
- a published website at `https://YOUR_USERNAME.github.io/bio196-personal-website/`
- a customized homepage with your name and short introduction
- at least one edited content page
- no private, sensitive, or large raw data uploaded

## Start here

1. Click **Fork** on this repository.
2. Choose your own GitHub account as the owner.
3. Rename your fork:

   ```text
   bio196-personal-website
   ```

4. Make sure you are editing the `source` branch.
5. Customize the website files.
6. Publish with GitHub Pages using GitHub Actions.
7. Submit both links:

   - your GitHub repository link
   - your published website link

## Files you will edit first

Start with these files:

| File or folder | What it controls |
| --- | --- |
| `_config.yml` | Your name, site title, links, navigation, and site settings |
| `_pages/` | Markdown pages such as home, about, research, teaching, or software |
| `images/` | Profile photo or other website images |
| `assets/ref.bib` | Optional bibliography file if you want to list publications |

You do not need to understand every file in the template before starting. Begin with `_config.yml` and one page in `_pages/`.

## Optional: preview the website on your computer

You do not need to install Ruby, Jekyll, or Node.js for the simplest version of this assignment. GitHub Actions can build the website online after you push to GitHub.

Local preview is useful if:

- you want to check the website before pushing
- GitHub Pages fails and you need to troubleshoot
- you are the instructor preparing the course template
- you want to make larger design changes

To preview locally, you need Ruby and Jekyll. Follow the Jekyll installation guide for your operating system:

```text
https://jekyllrb.com/docs/installation/
```

Then run:

```bash
bundle install
bundle exec jekyll serve
```

Open the local address printed in the terminal. It is often:

```text
http://localhost:4000
```

If this template uses a project-site `baseurl`, the local preview may instead be under:

```text
http://localhost:4000/bio196-personal-website/
```

Node.js packages are only needed if you plan to edit and rebuild the JavaScript:

```bash
npm install
```

## Publish with GitHub Pages

This template uses GitHub Actions to build the website.

After you fork and customize the repository:

1. Open your fork on GitHub.
2. Go to **Settings**.
3. Go to **Pages**.
4. Under **Source**, choose **GitHub Actions**.
5. Wait a few minutes for the site to build.

Your website link should look like:

```text
https://YOUR_USERNAME.github.io/bio196-personal-website/
```

## What to submit

Submit:

```text
Repository link:
https://github.com/YOUR_USERNAME/bio196-personal-website

Website link:
https://YOUR_USERNAME.github.io/bio196-personal-website/
```

## Privacy and data rules

Do not upload:

- private data
- controlled-access data
- passwords or tokens
- private SSH keys
- unpublished sensitive work
- large raw sequencing files such as FASTQ, BAM, or CRAM files

Use small public example files only if the assignment asks for data.

## Credit

This course template is adapted from an academic website template by the original template authors. The original template included broader documentation for academic and research group websites; this README has been simplified for BIO196 students.

## License

MIT


# Original Template
You can check later if you would like to develop a true personal website and learn more about the original project. 

## Features

### Design
- **Source Serif 4 + DM Sans** typography — elegant serif headings paired with a clean geometric sans body
- **Warm parchment palette** with subtle noise texture for depth, not flat generic whites
- **Dark mode** — toggle in navbar, auto-detects system preference, persists across visits
- **Frosted glass navbar** with backdrop blur, active page indicator, and scroll shadow
- **Dynamic SVG favicon** — auto-generated from your initials + accent color
- **Responsive** — CSS Grid layouts that adapt from desktop to tablet to mobile

### Interactions
- **Site-wide search** — press `Cmd+K` (or `Ctrl+K`) to instantly search all pages
- **Copy BibTeX** — hover any bibtex block to reveal a one-click copy button
- **Animated link underlines** — smooth gradient underlines that grow on hover
- **Card hover effects** — lift + shadow on team cards, research cards, and profile photo
- **Image zoom** — subtle scale on hover for team photos, research thumbnails, and the banner
- **Back-to-top button** — appears on scroll, smooth scrolls up
- **Smooth expand/collapse** — CSS transitions on publication abstracts and BibTeX entries

### Publications
- **Auto-generated from BibTeX** via Jekyll Scholar — just edit `assets/ref.bib`
- **Search bar** — filter publications by title, author, or year
- **Year badges** — small accent-colored pills for quick scanning
- **Pill buttons** — PDF, DOI, arXiv, BIB, Abstract

### For New Users
- **Interactive setup script** — run `./setup.sh` to fill in your name, title, and institution
- **4-step `_config.yml`** — numbered sections with inline comments guide you through setup
- **Well-commented data files** — every field in `_data/*.yml` is explained with examples
- **Smart link handling** — empty links in config are automatically hidden (no broken icons)

### Technical
- **Modular SASS** — organized into `base/`, `components/`, `layouts/`, `utilities/`
- **Selective Bootstrap 5.3.3** — only imports the modules used, not the full bundle
- **Single JS file** (4KB minified) — dark mode, search, toggles, scroll effects, copy button
- **Auto-generated sitemap** via `jekyll-sitemap`
- **Open Graph + Twitter Cards** — links look good when shared on social media
- **MathJax 3** — LaTeX formula rendering out of the box

## Screenshots

| | |
|:---:|:---:|
| ![Publications](images/screenshots/publications.png) | ![Team](images/screenshots/team.png) |
| Publications with search & year badges | Team page with card grid |
| ![Search](images/screenshots/search.png) | |
| Site-wide search (Cmd+K) | |

## Quick Start

1. **Fork** [this repository](https://github.com/sbryngelson/academic-website-template)
2. **Delete** `_config_demo.yml` (it's only for the demo site)
3. **Install** [Jekyll](https://jekyllrb.com/docs/installation/) and run `bundle install`
3. **Configure** your site:
   ```bash
   ./setup.sh          # interactive setup, or
   vim _config.yml     # edit Steps 1-4 directly
   ```
4. **Add your publications** to `assets/ref.bib`
5. **Customize** data files in `_data/` (team members, news, awards, etc.)
6. **Preview** your site:
   ```bash
   bundle exec jekyll serve
   # open http://localhost:4000
   ```

## Detailed How-To Guide

### Step 1: Fork and Clone

```bash
# Fork the repo on GitHub, then clone your fork
git clone https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
cd YOUR_USERNAME.github.io
```

### Step 2: Install Dependencies

You need Ruby and Jekyll installed. See [Jekyll's installation guide](https://jekyllrb.com/docs/installation/).

```bash
# Install Ruby gems
bundle install

# Optional: install Node.js dependencies (only needed if you want to edit JS)
npm install
```

### Step 3: Configure Your Identity

Open `_config.yml` and fill in your information. The file is organized into numbered steps:

```yaml
# STEP 1: Your Identity
name: "Jane Smith"
title: "Assistant Professor of Computer Science"
institution: "Stanford University"
email: jsmith@stanford.edu
photo: headshot.jpg   # place your photo in images/
```

Or run the interactive setup script:

```bash
./setup.sh
```

### Step 4: Add Your Links

Still in `_config.yml`, add your academic profiles. Delete any you don't use:

```yaml
# STEP 2: Your Links
links:
  google_scholar: "https://scholar.google.com/citations?user=YOUR_ID"
  github: "https://github.com/yourusername"
  orcid: "https://orcid.org/0000-0000-0000-0000"
  cv: "papers/cv.pdf"        # place your CV in the papers/ directory
  twitter: ""                # leave blank to hide
  linkedin: ""
```

### Step 5: Add Your Photo

Place your profile photo in the `images/` directory. Update the `photo` field in `_config.yml` to match the filename.

### Step 6: Add Publications

Edit `assets/ref.bib` with your BibTeX entries. The publications page is auto-generated. Example:

```bibtex
@article{smith2024,
  author = {Smith, Jane and Doe, John},
  title = {A Novel Approach to Machine Learning},
  journal = {Nature},
  year = {2024},
  volume = {42},
  pages = {1--10},
  doi = {10.1234/example},
  file = {smith2024.pdf},       % place PDF in papers/
  abstract = {We present...}
}
```

To bold your name in the publication list, update the scholar settings in `_config.yml`:

```yaml
scholar:
  last_name: Smith
  first_name: [Jane, J.]
```

Then uncomment the name-bolding line in `_layouts/bibtemplate.html`.

### Step 7: Add Team Members

Edit `_data/team_members.yml`:

```yaml
- name: Alice Johnson
  photo: alice.jpg          # place in images/ or images/team/
  info: PhD Student, started Fall 2023
  email: alice@university.edu
  website: https://alice.dev
  github: https://github.com/alice
```

### Step 8: Add News

Edit `_data/news.yml` (newest first):

```yaml
- date: 15 March, 2024
  headline: "Our paper on X was accepted to NeurIPS!"

- date: 1 January, 2024
  headline: "Welcome to new PhD student Alice Johnson"
```

### Step 9: Customize Pages

Each page in `_pages/` is a Markdown file. Edit the content directly:

- `home.md` — your welcome text and bio
- `research.md` — describe your research areas
- `software.md` — list your software projects
- `teaching.md` — list your courses

To remove a page from the navbar, comment it out in `_config.yml`:

```yaml
nav_pages:
  - name: about
  - name: publications
  # - name: talks        # hidden from navbar
  - name: research
```

### Step 10: Preview and Deploy

```bash
# Preview locally
bundle exec jekyll serve
# Visit http://localhost:4000

# When ready, push to GitHub
git add -A
git commit -m "My academic website"
git push
```

A GitHub Actions workflow automatically builds and deploys your site on every push. Make sure to go to **Settings > Pages > Source** in your repo and select **GitHub Actions**.

Your site will be live at `https://YOUR_USERNAME.github.io` within a few minutes.

---

## Customization

### _config.yml

The config file is organized into 4 numbered steps:

| Step | Section | What to fill in |
|------|---------|-----------------|
| 1 | **Your Identity** | Name, title, institution, email, photo |
| 2 | **Your Links** | Google Scholar, GitHub, ORCID, Twitter, LinkedIn, CV |
| 3 | **Site Settings** | Accent color, dark mode toggle, analytics |
| 4 | **Your Pages** | Comment out any pages you don't need |

### Data Files

| File | Purpose |
|------|---------|
| `_data/team_members.yml` | Current students and postdocs |
| `_data/alumni.yml` | Former lab members |
| `_data/news.yml` | News items (3 most recent shown on home) |
| `_data/awards.yml` | Awards and honors |
| `_data/grants.yml` | Grants and funding |
| `_data/funders.yml` | Funder logos |
| `_data/people.yml` | Students and mentees |
| `_data/pi.yml` | Optional: detailed education for About page |

Each file has inline comments explaining every field. Entries marked `# EXAMPLE` should be replaced or deleted.

### Pages

All pages are in `_pages/`. Edit the Markdown content directly. Pages use the `gridlay` layout by default.

### Accent Color & Dark Mode

Set `accent_color` in `_config.yml` to change the theme color across the entire site (links, buttons, highlights, favicon). Set `dark_mode: false` to disable the dark mode toggle entirely.

### CSS & JS Customization

The site uses modular SASS in `_sass/`:

```
_sass/
  base/          # variables, typography, reset
  components/    # card, navbar, buttons, footer, profile, publication, search
  layouts/       # home grid, team grid, research grid
  utilities/     # dark mode, animations
```

For JavaScript, edit `assets/js/site.js` then run `npm run build` to minify. Pre-built JS is committed, so `npm` is only needed if you modify the source.

## Publications

Publications are managed via [Jekyll Scholar](https://github.com/inukshuk/jekyll-scholar) using BibTeX. Edit `assets/ref.bib` with your references.

Update `scholar.last_name` and `scholar.first_name` in `_config.yml` to auto-bold your name in the publication list.

## Hosting

### GitHub Pages

Fork this repo as `your_username.github.io` and push. A **GitHub Actions workflow** is included (`.github/workflows/deploy.yml`) that automatically builds the site with Jekyll Scholar and deploys to GitHub Pages on every push to `source`.

To enable it: go to your repo's **Settings > Pages > Source** and select **GitHub Actions** instead of "Deploy from a branch".

### Custom Domain

Purchase a domain, update the `CNAME` file, and configure DNS. See [GitHub's guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

### Self-Hosting

Build with `bundle exec jekyll serve`, then upload `_site/` to your server. Set `url` and `baseurl` in `_config.yml` accordingly.

## Upgrading

Coming from the previous version? See [UPGRADING.md](UPGRADING.md).

## Alternatives

* [al-folio](https://github.com/alshedivat/al-folio)
* [academicpages](https://academicpages.github.io/)
* [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)

## Acknowledgment

I credit the [Allen Lab](https://www.allanlab.org/) for creating a beautiful academic research group webpage. Many parts of this site were adopted or copied from their laboratory webpage.

## License

MIT
