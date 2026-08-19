# Scalable QEC Workshop 2026 website template

This repository is a simple Jekyll/GitHub Pages website for the Scalable Quantum Error Correction Workshop 2026.

## The files you will normally edit

### 1. Speaker information
Edit:

`docs/_data/speakers.yml`

For each speaker, enter:
- name
- affiliation
- photo filename
- personal/professional website
- talk title
- abstract
- short bio

Add the corresponding photograph to:

`docs/assets/images/speakers/`

For best results, use portrait or headshot images of roughly the same aspect ratio. JPG, PNG, and WebP all work; make the filename in `speakers.yml` match the actual image.

### 2. Program / schedule
Edit:

`docs/_data/schedule.yml`

For talks, point `speaker:` to the speaker's `id` from `speakers.yml`. This automatically inserts the speaker name, affiliation, and talk title into the schedule.

### 3. Date, venue, workshop description, topics, organizers
Edit:

`docs/index.html`

The date/location are currently placeholders. The organizer names and affiliations are also placeholders.

### 4. Header date/location and contact email
Edit:

`docs/_layouts/default.html`

Change `September XX, 2026`, `Location · City, State`, and `contact@example.com`.

## Add more speakers

Copy one complete entry in `docs/_data/speakers.yml`, give the new speaker a unique `id`, and add the corresponding image. Then add a `type: talk` entry to `docs/_data/schedule.yml` if the talk should appear in the schedule.

## Publish on GitHub Pages

1. Create a repository named `QECWorkshop2026` under the `Error-Correction-Lab` organization.
2. Upload/push these files.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/docs`.
6. Save.

The site should then be available at:

`https://error-correction-lab.github.io/QECWorkshop2026/`

The `_config.yml` in this template already uses `/QECWorkshop2026` as the base URL.

## Custom domain

This template deliberately does **not** include a `CNAME` file. Add one only if you intentionally want to use a custom domain for the 2026 workshop.
