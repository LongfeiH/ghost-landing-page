# Ghost Landing Page
## Ghost
&nbsp;
<p align="center">
  <a href="https://ghost.org/#gh-light-mode-only" target="_blank">
    <img src="https://user-images.githubusercontent.com/65487235/157884383-1b75feb1-45d8-4430-b636-3f7e06577347.png" alt="Ghost" width="200px">
  </a>
  <a href="https://ghost.org/#gh-dark-mode-only" target="_blank">
    <img src="https://user-images.githubusercontent.com/65487235/157849205-aa24152c-4610-4d7d-b752-3a8c4f9319e6.png" alt="Ghost" width="200px">
  </a>
</p>
&nbsp;

<p align="center">
    <a href="https://ghost.org/">Ghost.org</a> •
    <a href="https://forum.ghost.org">Forum</a> •
    <a href="https://ghost.org/docs/">Docs</a> •
    <a href="https://github.com/TryGhost/Ghost/blob/main/.github/CONTRIBUTING.md">Contributing</a> •
    <a href="https://twitter.com/ghost">Twitter</a>
    <br /><br />
    <a href="https://ghost.org/">
        <img src="https://img.shields.io/badge/downloads-3M-brightgreen.svg" alt="Downloads" />
    </a>
    <a href="https://github.com/TryGhost/Ghost/releases/">
        <img src="https://img.shields.io/github/release/TryGhost/Ghost.svg" alt="Latest release" />
    </a>
    <a href="https://github.com/TryGhost/Ghost/actions">
        <img src="https://github.com/TryGhost/Ghost/workflows/CI/badge.svg?branch=main" alt="Build status" />
    </a>
    <a href="https://github.com/TryGhost/Ghost/contributors/">
        <img src="https://img.shields.io/github/contributors/TryGhost/Ghost.svg" alt="Contributors" />
    </a>
</p>

&nbsp;

<a href="https://ghost.org/"><img src="https://user-images.githubusercontent.com/353959/169805900-66be5b89-0859-4816-8da9-528ed7534704.png" alt="Fiercely independent, professional publishing. Ghost is the most popular open source, headless Node.js CMS which already works with all the tools you know and love." /></a>

&nbsp;

Ghost is a popular open-source content management system (CMS) and blogging platform. Designed to be simple, elegant, and focused solely on publishing content, Ghost provides a user-friendly interface for writers and bloggers to create and manage their posts effortlessly.

This repository aims to leverage Ghost to swiftly and efficiently build a stunning landing-page website and deploy it using Amplify.

If you want to know more about ghost, you can click the picture above or the ghost icon to jump to the ghost home page

&nbsp;

## Amplify
&nbsp;

Amplify is a cloud development platform that enables seamless and scalable deployment of web and mobile applications. 

With Amplify, developers can quickly set up, manage, and automate the entire application deployment process, making it easier to focus on building and enhancing the core functionalities of their applications without worrying about server infrastructure.

If you have an AWS account, you can click <a href="https://ap-southeast-1.console.aws.amazon.com/">here</a> to access the AWS console and explore Amplify in more detail.

Amplify can deploy various types of websites, including static websites, single-page applications (SPAs), and serverless web applications. However, it cannot directly deploy Ghost, which is a dynamic content management system (CMS) and requires a server to run. 

So we need a tool to generate static sites for ghost.

&nbsp;

## Ghost Static Site Generator
&nbsp;

This is a static site generation tool specially designed for ghost and based on wget. It is very convenient to use. When your ghost project is running on the localhost:2368 endpoint, you only need to enter `gssg` in the terminal, and the corresponding static website file will be generated in the current folder

If you want to know more about `gssg`, please click <a href="https://github.com/Fried-Chicken/ghost-static-site-generator">here</a>.


&nbsp;

## How to Contribute

1. First, clone the repository:
    ```
    git init
    git clone git@github.com:ocademy-ai/ghost-landing-page.git
    ```
2. Install dependencies
   ```
   yarn install
   ```
   If you have not installed yarn, please install it first
3. Start server
   ```
   yarn run dev
   ```
4. Make some changes   
     
   Open localhost:2368 and make some changes.
5. Commit changes  
     
   Push commit or submit a pull request to synchronize your local changes to the main branch.

**Note1:** You don't need to run gssg yourself to generate the static site, once the main branch has any commits, github actions will run gssg to generate the static site files according to the latest change records, and upload them all to the gh-pages branch. If you want to understand the whole process, please check the `.github/workflows/main.yml` file

**Note2:** Do not make any changes to the gh-pages branch, it is a clean, static site file storage branch, and it is associated with amplify, any changes to the gh-pages branch will cause the site to be re-deployed.

## Verify changes

Finally, if you want to visit the deployed website to verify your changes, please click <a href="https://gh-pages.d2iqc9095blb4x.amplifyapp.com/">here</a>.

Username: ocademy2023
Password: q7ZMwiZzQHjeH5X