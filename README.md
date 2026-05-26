# 🟩 Auto Commit Green Profile

> 🌳 Keeping the GitHub contribution graph green — every 4 hours, automatically!
> Powered by [GitHub Actions](https://github.com/features/actions)

[![Auto Commit](https://github.com/BarzzLy/Auto-Commit-Green-Profile/workflows/Auto%20Commit%20Green%20Profile/badge.svg)](https://github.com/BarzzLy/Auto-Commit-Green-Profile/actions)

---

## 🚀 How It Works

This repo uses a **GitHub Actions workflow** that runs automatically every **4 hours**.

Each run:
1. ✅ Checks out the repository
2. 📝 Updates the `LAST_UPDATED` file with the current timestamp
3. 💬 Creates a commit with a random fun emoji message
4. 🚀 Pushes the commit to keep the contribution graph active

---

## ⚙️ Setup (for others who want to use this)

1. **Fork or use this template** — Click "Use this template" (⚠️ forked repos won't trigger the workflow)
2. **Enable workflow permissions** — Go to: `Settings` → `Actions` → `General` → `Workflow permissions` → Select **"Read and write permissions"**
3. **Update your identity** in `.github/workflows/autocommit.yml`:
   ```yaml
   git config --local user.email "your@email.com"
   git config --local user.name "YourGitHubUsername"
   ```
4. **Adjust the schedule** if needed — default is every 4 hours (`0 */4 * * *`)
5. ✅ Done! The workflow will start running on the next scheduled trigger.

---

## 🗓️ Schedule

| Trigger | Description |
|---|---|
| ⏰ Schedule | Every 4 hours (`0 */4 * * *`) |
| 📤 Push | On every push to `main` / `master` |
| 🖱️ Manual | Can be triggered manually via GitHub Actions UI |

---

## 🛠️ Tech Stack

- [GitHub Actions](https://github.com/features/actions)
- [ad-m/github-push-action](https://github.com/ad-m/github-push-action)

---

## 👤 Author

Made with 💚 by **[BarzzLy](https://github.com/BarzzLy)**
