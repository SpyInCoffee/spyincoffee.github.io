---
title: Hello, World.
date: 2024-10-18
tags: [tutorial]     # TAG names should always be lowercase
---

## What to Expect from This Blog

Before diving into the technical aspects of how this site was deployed, I’d like to provide a brief overview of what you can expect from future posts:

### Topics Covered:

- **Client Projects**: These will be anonymized unless highlighted as specific case studies.
- **Side Projects**: Detailed technical walkthroughs of personal or exploratory projects.
- **Scripts**: Custom scripts I've developed, along with real-world use cases and applications.
- **Industry Insights**: Including updates, trends, and interviews with professionals from the field.

To stay informed about future updates, feel free to subscribe via the [RSS feed](https://spyincoffee.github.io/feed.xml) or connect on [LinkedIn](https://www.linkedin.com/in/lukasroberts/).


> Below is a short guide on how I deployed this Jekyll site via GitHub Pages. It's an extension of this "Hello, World!" page, in case anyone is inspired to set up something similar. The following is a condensed version of the official documentation, and I highly recommend diving deeper into [Jekyll](https://jekyllrb.com/) and the [Chirpy theme](https://github.com/cotes2020/jekyll-theme-chirpy) for further infomration.
{: .prompt-info }

## Deploying a Jekyll Static Site

### Environment Setup

- **Operating System**: Windows 11
- **Tools Required**:
  - Docker Desktop
  - Visual Studio Code (VS Code)
  - Dev Containers extension for VS Code
  - GitHub account

> Don't forget to share your Git credentials with your container. For detailed instructions, refer to the [Sharing Git Credentials with Your Container](https://code.visualstudio.com/remote/advancedcontainers/sharing-git-credentials) guide.
{: .prompt-info }

## Using the Chirpy Starter Template

This guide provides an overview of how to install, configure, and use a Jekyll theme, and ultimately deploy it to a web server.

### Using the Starter

This method simplifies future updates, isolates unnecessary files, and is ideal for users who prefer minimal configuration.

1. Sign in to GitHub and navigate to the theme's repository.
2. Name your new repository `<username>.github.io`, replacing `username` with your lowercase GitHub username.

### Using Dev Containers

Dev Containers create an isolated environment using Docker, preventing conflicts with your local system and ensuring all dependencies are managed within the container.

1. **Install Docker**:
   - On Windows/macOS, install **Docker Desktop**.
2. **Install VS Code** and the **Dev Containers extension**.
3. **Clone your repository**:
   - Open VS Code and [clone your repository within a container volume](https://code.visualstudio.com/docs/devcontainers/containers#:~:text=Start%20VS%20Code%20and%20run,that%20appears%20and%20press%20Enter.).

4. Wait for the Dev Containers setup to complete.

### Usage

To start your Jekyll server, run the following command in a VS terminal:

```terminal
$ bundle exec jekyll s
```
After your site is running, make required changes, apply your staged changes, commit them, and push them to GitHub for deployment.

> If you experience any issues while pushing updates from a branch, update the build and deployment source to GitHub Actions. After making this change, re-run all jobs under the Pages Actions.
>{: .prompt-warning }
