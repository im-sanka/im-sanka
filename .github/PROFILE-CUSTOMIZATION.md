# GitHub Profile Customization Guide

## Overview

Your GitHub profile now features a modern, dynamic README that automatically updates daily with your latest activity.

## Features

### 1. **Dynamic GitHub Statistics**
- GitHub stats card showing your contributions, stars, PRs, and issues
- Top languages card displaying your most used programming languages
- Streak stats showing your contribution streak

### 2. **Recent Activity**
- Automatically updates daily at midnight UTC
- Shows your latest GitHub activities (commits, PRs, issues, stars, etc.)
- Updates are powered by a GitHub Actions workflow

### 3. **Tech Stack Display**
- Customizable badges for languages and tools you use
- Visual representation of your skills

### 4. **GitHub Trophies**
- Achievement showcase based on your GitHub activity

### 5. **Contribution Graph**
- Visual representation of your contribution activity over time

### 6. **Profile Views Counter**
- Tracks how many people have viewed your profile

## Customization

### Update Your Name and Title

Edit the header section in `README.md`:
```markdown
# 👋 Hello, I'm Sanka!
### 🚀 Developer | Builder | Creator
```

### Update Tech Stack

Modify the tech stack section to reflect your actual skills:
```markdown
## 💻 Tech Stack
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
```

Visit [shields.io](https://shields.io) to create custom badges.

### Update Social Links

Update your social media links in the "Connect With Me" section:
```markdown
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_USERNAME)
```

### Customize Themes

All stats use the `tokyonight` theme. Available themes include:
- `dark`
- `radical`
- `merko`
- `gruvbox`
- `tokyonight`
- `onedark`
- `cobalt`
- `synthwave`
- `highcontrast`
- `dracula`

Change the theme parameter in the URL, e.g.:
```
?theme=dracula
```

## Workflow Configuration

The GitHub Actions workflow (`.github/workflows/update-readme.yml`) runs:
- Daily at midnight UTC
- On every push to the main branch
- Manually via workflow dispatch

### Manual Trigger

You can manually trigger the workflow from:
1. Go to the "Actions" tab in your repository
2. Select "Update README" workflow
3. Click "Run workflow"

## How It Works

1. The workflow uses GitHub's API to fetch your recent activity
2. It parses events like commits, PRs, issues, stars, and forks
3. Updates the section between `<!-- ACTIVITY:START -->` and `<!-- ACTIVITY:END -->`
4. Commits the changes back to the repository

## Troubleshooting

### Activity not updating?
- Check the Actions tab for workflow run status
- Ensure the workflow has write permissions
- Verify the activity markers are present in README.md

### Stats not showing?
- The external services (github-readme-stats, streak-stats) need to be accessible
- They may have rate limits or temporary outages
- Wait a few minutes and refresh

## Resources

- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [GitHub Readme Streak Stats](https://github.com/DenverCoder1/github-readme-streak-stats)
- [GitHub Profile Trophy](https://github.com/ryo-ma/github-profile-trophy)
- [Shields.io](https://shields.io)
- [Simple Icons](https://simpleicons.org) - For badge logos

## Contributing

Feel free to customize this profile to match your personal brand and style!
