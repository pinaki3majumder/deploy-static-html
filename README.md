# Basic CI Workflow for Static HTML/CSS/JS Using GitHub Actions
This repository demonstrates how to set up a simple Continuous Integration (CI) workflow using [GitHub Actions](https://docs.github.com/en/actions) for a static website with HTML, CSS, and JavaScript.

## Prerequisites
- A GitHub repository containing your static HTML, CSS, and JS files.
- Basic knowledge of GitHub Actions, YAML syntax, and Git commands.

## A Step-By-Step Guide

**Step 1 :** Create an Empty GitHub Repository

**Step 2 :** Clone the Repository

**Step 3 :** Add a basic HTML file with some texts.

**Step 4 :** Commit and Push the changes.

**Step 5 :** Open the `settings` of your repository and go to `Pages`.

- From the `source` select `GitHub Actions`. (This will allow us to deploy our code using GitHub Actions which will create CI workflow.)

**Step 6 :** Click on `Configure` button from Static HTML card/section.
    
    
- This will generate a pre-build workflow for static HTML file.
- The following image is the workflow YAML file that will automate the deployment process.

- This files contains:

    - `name`: Name of your workflow
    - `on`: Action from which you to automate your task
    - `permission`: Here we provide permissions to read, write our workflow files.
    - `jobs`: This is where your mention all the task you want to automate.

**Step 7 :** From the above repo tabs go to `Actions` and check if your app is deployed on Github Pages or not. Open the deployment by clicking on the workflow name.

**Step 8 :** Go to the link provided by GitHub this is where your HTML file is deployed.

**Step 9 :** After opening the link you can see the contents of your HTML file.

**Step 10 :** Now let's check if CI workflow or not. First, pull your changes.

- Modify your code and push it on the GitHub.
- Wait for 10-15 seconds and reload your site. The new changes will appear on the site.


## Automated CI/CD Workflow - FlowChart

<svg width="200px" height="200px" viewBox="0 0 1024 1024" class="icon"  version="1.1" xmlns="http://www.w3.org/2000/svg"><path d="M741.7 844.4H282.3c-17.4 0-31.5-14.1-31.5-31.5V211.1c0-17.4 14.1-31.5 31.5-31.5h459.4c17.4 0 31.5 14.1 31.5 31.5v601.8c0 17.4-14.1 31.5-31.5 31.5z" fill="#68A240" /><path d="M741.7 849.9H282.3c-20.4 0-37-16.6-37-37V211.1c0-20.4 16.6-37 37-37h459.4c20.4 0 37 16.6 37 37v601.8c0 20.4-16.6 37-37 37zM282.3 185.1c-14.3 0-26 11.7-26 26v601.8c0 14.3 11.7 26 26 26h459.4c14.3 0 26-11.7 26-26V211.1c0-14.3-11.7-26-26-26H282.3z" fill="#333336" /><path d="M697.9 349.3s15.6 40.8-159.2 40.8c-178.6 0-220-40.8-220-40.8v-96.9c0-6.4 5.5-11.6 12.3-11.6h354.5c6.8 0 12.3 5.2 12.3 11.6v96.9z" fill="#FFD632" /><path d="M538.7 395.6c-178.8 0-222.1-40.6-223.8-42.4l-1.6-1.6v-99.2c0-9.4 8-17.1 17.8-17.1h354.5c9.8 0 17.8 7.7 17.8 17.1v96.2c0.5 2.4 1 8-3.4 14.4-14.7 21.4-70.5 32.6-161.3 32.6z m-214.4-48.9c4 3 15.9 10.7 40.8 18.2 29.4 9 83.4 19.6 173.7 19.6 120.1 0 146.4-19.5 152.2-27.8 2.2-3.2 1.8-5.5 1.8-5.5l-0.4-0.9v-97.9c0-3.4-3-6.1-6.8-6.1H331.1c-3.7 0-6.8 2.7-6.8 6.1v94.3z" fill="#333336" /><path d="M575 310.4h-6.9c-2.8 0-5.1-2.3-5.1-5.1V277c0-2.8 2.3-5.1 5.1-5.1h6.9c2.8 0 5.1 2.3 5.1 5.1v28.2c0 2.9-2.3 5.2-5.1 5.2zM575 356.4h-6.9c-2.8 0-5.1-2.3-5.1-5.1V323c0-2.8 2.3-5.1 5.1-5.1h6.9c2.8 0 5.1 2.3 5.1 5.1v28.2c0 2.9-2.3 5.2-5.1 5.2zM652.9 318.9h-41.6c-2.4 0-4.3-1.9-4.3-4.3v-5.8c0-2.4 1.9-4.3 4.3-4.3h41.6c2.4 0 4.3 1.9 4.3 4.3v5.8c0 2.4-1.9 4.3-4.3 4.3z" fill="#333336" /><path d="M639.7 292.5v38.4c0 2.5-2 4.5-4.5 4.5h-6.1c-2.5 0-4.5-2-4.5-4.5v-38.4c0-2.5 2-4.5 4.5-4.5h6.1c2.5 0 4.5 2 4.5 4.5z" fill="#333336" /><path d="M432.9 504.6H353c-18.9 0-34.2-15.3-34.2-34.2v-3.1c0-18.9 15.3-34.2 34.2-34.2h79.8c18.9 0 34.2 15.3 34.2 34.2v3.1c0.1 18.9-15.2 34.2-34.1 34.2z" fill="#D5D9CF" /><path d="M432.9 510.1H353c-21.9 0-39.7-17.8-39.7-39.7v-3.1c0-21.9 17.8-39.7 39.7-39.7h79.8c21.9 0 39.7 17.8 39.7 39.7v3.1c0.1 21.9-17.7 39.7-39.6 39.7zM353 438.5c-15.9 0-28.7 12.9-28.7 28.7v3.1c0 15.9 12.9 28.7 28.7 28.7h79.8c15.9 0 28.7-12.9 28.7-28.7v-3.1c0-15.9-12.9-28.7-28.7-28.7H353z" fill="#333336" /><path d="M318.8 468.8a37.9 35.8 0 1 0 75.8 0 37.9 35.8 0 1 0-75.8 0Z" fill="#FFD632" /><path d="M356.7 510.1c-23.9 0-43.4-18.5-43.4-41.3s19.5-41.3 43.4-41.3 43.4 18.5 43.4 41.3-19.5 41.3-43.4 41.3z m0-71.6c-17.8 0-32.4 13.6-32.4 30.3s14.5 30.3 32.4 30.3 32.4-13.6 32.4-30.3-14.5-30.3-32.4-30.3z" fill="#333336" /><path d="M485.8 650.4H333.4c-8.1 0-14.6-6.5-14.6-14.6v-58.3c0-8.1 6.5-14.6 14.6-14.6h152.3c8.1 0 14.6 6.5 14.6 14.6v58.3c0 8.1-6.5 14.6-14.5 14.6z" fill="#FFD632" /><path d="M485.8 655.9H333.4c-11.1 0-20.1-9-20.1-20.1v-58.3c0-11.1 9-20.1 20.1-20.1h152.3c11.1 0 20.1 9 20.1 20.1v58.3c0 11.1-9 20.1-20 20.1z m-152.4-87.5c-5 0-9.1 4.1-9.1 9.1v58.3c0 5 4.1 9.1 9.1 9.1h152.3c5 0 9.1-4.1 9.1-9.1v-58.3c0-5-4.1-9.1-9.1-9.1H333.4z" fill="#333336" /><path d="M485.8 788.1H333.4c-8.1 0-14.6-6.5-14.6-14.6v-58.3c0-8.1 6.5-14.6 14.6-14.6h152.3c8.1 0 14.6 6.5 14.6 14.6v58.3c0 8-6.5 14.6-14.5 14.6z" fill="#FFD632" /><path d="M485.8 793.6H333.4c-11.1 0-20.1-9-20.1-20.1v-58.3c0-11.1 9-20.1 20.1-20.1h152.3c11.1 0 20.1 9 20.1 20.1v58.3c0 11.1-9 20.1-20 20.1z m-152.4-87.5c-5 0-9.1 4.1-9.1 9.1v58.3c0 5 4.1 9.1 9.1 9.1h152.3c5 0 9.1-4.1 9.1-9.1v-58.3c0-5-4.1-9.1-9.1-9.1H333.4z" fill="#333336" /><path d="M682.8 786.6H577c-7.7 0-13.9-6.2-13.9-13.9v-194c0-7.7 6.2-13.9 13.9-13.9h105.9c7.7 0 13.9 6.2 13.9 13.9v194c-0.1 7.7-6.3 13.9-14 13.9z" fill="#D8A128" /><path d="M682.8 792.1H577c-10.7 0-19.4-8.7-19.4-19.4v-194c0-10.7 8.7-19.4 19.4-19.4h105.9c10.7 0 19.4 8.7 19.4 19.4v194c-0.1 10.7-8.8 19.4-19.5 19.4zM577 570.3c-4.7 0-8.4 3.8-8.4 8.4v194c0 4.7 3.8 8.4 8.4 8.4h105.9c4.7 0 8.4-3.8 8.4-8.4v-194c0-4.7-3.8-8.4-8.4-8.4H577z" fill="#333336" /><path d="M539.1 456.5l-15.2 27.9" fill="#D8A128" /><path d="M523.8 489.9c-0.9 0-1.8-0.2-2.6-0.7-2.7-1.5-3.7-4.8-2.2-7.5l15.2-27.9c1.5-2.7 4.8-3.6 7.5-2.2 2.7 1.5 3.7 4.8 2.2 7.5L528.7 487c-1 1.8-2.9 2.9-4.9 2.9z" fill="#333336" /><path d="M579.1 456.5l-15.2 27.9" fill="#D8A128" /><path d="M563.9 489.9c-0.9 0-1.8-0.2-2.6-0.7-2.7-1.5-3.7-4.8-2.2-7.5l15.2-27.9c1.5-2.7 4.8-3.6 7.5-2.2 2.7 1.5 3.7 4.8 2.2 7.5L568.8 487c-1 1.8-2.9 2.9-4.9 2.9z" fill="#333336" /><path d="M619.2 456.5L604 484.4" fill="#D8A128" /><path d="M604 489.9c-0.9 0-1.8-0.2-2.6-0.7-2.7-1.5-3.7-4.8-2.2-7.5l15.2-27.9c1.5-2.7 4.8-3.6 7.5-2.2 2.7 1.5 3.7 4.8 2.2 7.5L608.9 487c-1 1.8-2.9 2.9-4.9 2.9z" fill="#333336" /><path d="M659.3 456.5l-15.2 27.9" fill="#D8A128" /><path d="M644.1 489.9c-0.9 0-1.8-0.2-2.6-0.7-2.7-1.5-3.7-4.8-2.2-7.5l15.2-27.9c1.5-2.7 4.8-3.6 7.5-2.2 2.7 1.5 3.7 4.8 2.2 7.5L649 487c-1 1.8-2.9 2.9-4.9 2.9z" fill="#333336" /><path d="M699.4 456.5l-15.2 27.9" fill="#D8A128" /><path d="M684.2 489.9c-0.9 0-1.8-0.2-2.6-0.7-2.7-1.5-3.7-4.8-2.2-7.5l15.2-27.9c1.5-2.7 4.8-3.6 7.5-2.2 2.7 1.5 3.7 4.8 2.2 7.5L689.1 487c-1 1.8-2.9 2.9-4.9 2.9z" fill="#333336" /></svg>
