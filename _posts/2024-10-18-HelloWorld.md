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


## Deploying a Jekyll Static Site.

# Environment Setup

- **Operating System**: Windows 11
- **Tools Required**:
  - Docker Desktop
  - Visual Studio Code (VS Code)
  - Dev Containers extension for VS Code
  - GitHub account

> Remember to share pass your Git credentials with your container. For guidance, refer to the [Sharing Git Credentials with Your Container](https://code.visualstudio.com/remote/advancedcontainers/sharing-git-credentials) documentation.
{: .prompt-info }

## Getting Started with jeykell themse

In this comprehensive overview, you will learn how to install, configure, and use a jekell themse, as well as how to deploy it to a web server.

### Using the Starter

This approach simplifies upgrades, isolates unnecessary files, and is perfect for users who want to focus on writing with minimal configuration.

1. Sign in to GitHub and navigate to the themse
2. Name the new repository `<username>.github.io`, replacing `username` with your lowercase GitHub username.

### Using Dev Containers

Dev Containers offer an isolated environment using Docker, preventing conflicts with your system and ensuring all dependencies are managed within the container.

1. **Install Docker**:
   - On Windows/macOS, install **Docker Desktop**.
2. **Install VS Code** and the **Dev Containers extension**.
3. **Clone your repository**:
   - Start VS Code and clone your repository in a container volume.
4. Wait for the Dev Containers setup to complete.

### Usage

To start your Jekyll server, run the following command in a terminal:

```terminal
$ bundle exec jekyll s
```
>  you must run that command in the VS Code Terminal if you are using Dev Containers
{: .prompt-info }

At this point, 

The final part is to apply staged changes, and commit and push to github
