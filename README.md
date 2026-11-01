# 🧊 GitHub 3D Profile Template

Turn your GitHub profile into a 3D contribution graph, an animated contribution snake and stats cards. It is free, updates itself every day, and takes about 10 minutes.

Made by **[♛ GÖKBÖRÜ AI](https://nauman804.github.io/Portofolio/)** (M. Nauman Anwar).

## What you get

| Feature | How it works |
|---|---|
| 🧊 3D contribution graph | GitHub Action that writes SVG files into your repo |
| 🐍 Contribution snake | GitHub Action that writes SVG files to an `output` branch |
| 📊 Stats and top languages cards | GitHub Action that writes `profile/stats.svg` and `profile/top-langs.svg` |

No paid tool and no outside server is needed when someone views your profile. The images live in your own repo.

## Files in this template

```
PROFILE_README_TEMPLATE.md   your profile README (copy it as README.md)
workflows/profile-3d.yml     makes the 3D graph
workflows/snake.yml          makes the snake
workflows/grs.yml            makes the stats cards
```

## Setup (about 10 minutes)

1. **Create your profile repo.** Go to <https://github.com/new>. The repository name must be exactly your GitHub username. Choose **Public** and tick **Add a README file**.
2. **Add your README.** Open the repo's `README.md`, click the pencil icon, delete the text, and paste the contents of `PROFILE_README_TEMPLATE.md`. Replace every `YOUR-USERNAME` with your GitHub username, then commit.
3. **Add the three workflow files.** In your repo click **Add file > Create new file**. In the name box type `.github/workflows/profile-3d.yml` (typing the slashes creates the folders). Paste the content of `workflows/profile-3d.yml` and commit. Repeat for `snake.yml` and `grs.yml`.
4. **Give Actions permission to write.** Go to **Settings > Actions > General > Workflow permissions**, choose **Read and write permissions**, and click **Save**.
5. **Run each workflow once.** Open the **Actions** tab. For **GitHub-Profile-3D-Contrib**, **Generate Snake** and **Update README cards**, click the workflow and then **Run workflow**. Wait one to two minutes for the green tick.
6. **Open your profile** at `github.com/YOUR-USERNAME` and hard refresh with Ctrl+Shift+R.

## Troubleshooting

- **A broken image icon:** the workflow behind that image has not run yet, or it failed. Check the Actions tab for a red X and open it to read the error.
- **No `profile-3d-contrib` folder:** run the 3D workflow again after you set the write permission in step 4.
- **Snake missing:** it is read from the `output` branch, which is created the first time the snake workflow succeeds.
- **Only public repos are counted** by default. Private activity needs a personal access token and extra setup, see the tools' own docs.
- **Want a moving 3D graph?** In your README, change `profile-night-rainbow.svg` to `profile-green-animate.svg`.

## Credits

This template only combines these open-source tools. All credit for the tools goes to their authors.

- 3D graph: [yoshi389111/github-profile-3d-contrib](https://github.com/yoshi389111/github-profile-3d-contrib)
- Snake: [Platane/snk](https://github.com/Platane/snk)
- Stats cards: [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats) and its [Action](https://github.com/stats-organization/github-readme-stats-action)

Check each tool's page for its license.

## Need something built?

I build AI chatbots (RAG), automations with n8n and Make.com, AI websites and AI ads. Reach me through my [portfolio](https://nauman804.github.io/Portofolio/) or at maliknomangokboru@gmail.com.

## License

MIT, see [LICENSE](./LICENSE).
