# Setup & Push — GitHub Profile Repository

Your GitHub profile README only appears when the repository name matches your username exactly:

**Repository name must be:** `SkyLineCoderz-Raheel`

URL after push: `https://github.com/SkyLineCoderz-Raheel/SkyLineCoderz-Raheel`

---

## External services used

| Purpose | Service | URL pattern |
|---------|---------|-------------|
| Typing animation | [readme-typing-svg](https://github.com/DenverCoder1/readme-typing-svg) | `https://readme-typing-svg.demolab.com/...` |
| GitHub stats | [github-readme-stats](https://github.com/anuraghazra/github-readme-stats) | `https://github-readme-stats.vercel.app/api?username=SkyLineCoderz-Raheel` |
| Contribution streak | [github-readme-streak-stats](https://github.com/DenverCoder1/github-readme-streak-stats) | `https://streak-stats.demolab.com/?user=SkyLineCoderz-Raheel` |
| Top languages | github-readme-stats | `.../api/top-langs/?username=SkyLineCoderz-Raheel` |
| Badges | [shields.io](https://shields.io) | `https://img.shields.io/badge/...` |

All are HTTPS and commonly used in GitHub READMEs. Fallbacks are documented in the README stats `<details>` block and as a static title comment under the typing SVG.

No JavaScript. No unsupported CSS. No App Store Connect URLs.

---

## Before you push (checklist)

1. [ ] Replace SVG app icons with official PNGs (see `ASSETS.md`) — or keep SVGs temporarily  
2. [ ] Add `assets/profile/muhammad-raheel.png`  
3. [ ] Optional: export banner PNG and update README `src`  
4. [ ] Optional: set real CV URL on the CV badges  
5. [ ] Optional: add Ride Hailing store links when public  
6. [ ] Preview `README.md` locally (VS Code / Cursor Markdown preview)

---

## Git commands — create & push profile repo

Run from this folder (`/Applications/github_profile`).

### Option A — Create repo with GitHub CLI (recommended)

```bash
cd /Applications/github_profile

git init
git add README.md ASSETS.md SETUP.md assets
git commit -m "$(cat <<'EOF'
Add GitHub profile README for Muhammad Raheel.

Senior Flutter Tech Lead personal profile with projects, stack, and stats.
EOF
)"

gh repo create SkyLineCoderz-Raheel --public --source=. --remote=origin --push
```

If the empty profile repo already exists on GitHub:

```bash
cd /Applications/github_profile

git init
git add README.md ASSETS.md SETUP.md assets
git commit -m "$(cat <<'EOF'
Add GitHub profile README for Muhammad Raheel.

Senior Flutter Tech Lead personal profile with projects, stack, and stats.
EOF
)"

git branch -M main
git remote add origin https://github.com/SkyLineCoderz-Raheel/SkyLineCoderz-Raheel.git
git push -u origin main
```

### Option B — Manual remote

1. On GitHub: **New repository** → name exactly `SkyLineCoderz-Raheel` → Public → do **not** add a README  
2. Then:

```bash
cd /Applications/github_profile
git init
git add README.md ASSETS.md SETUP.md assets
git commit -m "$(cat <<'EOF'
Add GitHub profile README for Muhammad Raheel.

Senior Flutter Tech Lead personal profile with projects, stack, and stats.
EOF
)"
git branch -M main
git remote add origin https://github.com/SkyLineCoderz-Raheel/SkyLineCoderz-Raheel.git
git push -u origin main
```

---

## After pushing

1. Open `https://github.com/SkyLineCoderz-Raheel`  
2. Confirm the profile README renders under your bio  
3. Wait 1–2 minutes if stats images are blank (cold start on stats hosts)  
4. Pin important repos from your profile settings if desired  

---

## Updating later

```bash
cd /Applications/github_profile
# edit files / replace assets
git add -A
git commit -m "$(cat <<'EOF'
Update profile README assets and content.
EOF
)"
git push
```
