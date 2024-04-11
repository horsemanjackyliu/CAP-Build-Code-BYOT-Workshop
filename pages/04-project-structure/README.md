# Project structure, what is what

This repository contains everything you need to write your workshop so you can ignore most of the files, and concentrate in the content you want to show.

This project uses the web framework [Docsify](https://docsify.js.org/#/) (read more in their site), and is prepared to be deployed to SAP BTP Cloud Foundry. A quick walkthrough to the files and folders, by their function:

Where you will do most of the work:

- `pages/`: This is where you can [write your content](pages/05-writing-content): pages, exercises, etc
    - Inside, there is a folder for each page, and inside each folder:
        - `img/`: You can place images used in the page in the image folder
        - `files/`: You can place files used in the page in the image folder
        - `README.md`: This is where you write your page!
- `agenda-for-pdf.md`: This is where you control what will be added to the PDF
- `agenda-sidebar.md`: This is where you control the sidebar of the page

Docsify website framework (where you need to do one-time configurations):

- `_assets/`: Contains SAP branding files (logos and fonts). No need to touch this.
- `index.html`: The core configuration of the Docsify framework. Change only the [site title](pages/02-set-title/README.md) here

Deployment and other (no need to touch anything):

- `.gitignore`: Tells git and GitHub what files to ignore. No need to touch this.
- `manifest.json`: Makes the app available in SAP Build Workzone.
- `mta.yaml`: Instructions to prepare the app to be deployed in SAP BTP Cloud Foundry
- `package.json`: Project properties to be able to: run locally, build the website, prepare the PDF
- `xs-app.json`: SAP Build Workzone configuration for making the app available in SAP BTP
