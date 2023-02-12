# Curriculum Vitae

This was the result of an effort to automatically deploy the latest version of my CV to the internet. Neither the content nor the CI/CD steps are complicated.

## LaTeX Template

The CV itself was based off of a template that you can find [here](https://www.latextemplates.com/template/developer-cv) under the MIT License. All credits go to:

- Jan Vorisek (jan@vorisek.me)
- Based on a template by Jan Küster (info@jankuester.com)
- Modified for LaTeX Templates by Vel (vel@LaTeXTemplates.com)

I believe the same license should apply to this repository as well.

## Gitlab CI

The Gitlab CI Pipeline for this repo does the following steps:

- Compile the 'main.tex' file into a PDF called 'main.pdf' whenever you push to the 'main' branch
- Adds the PDF generated in the previous step and a basic redirect HTML file in a 'public' folder
- Uses the GITLAB action to publish a Gitlab pages page using the contents of the folder created above

## Fork This Repository

You can deploy your own CV by just forking this repository. You can find the link of the deployed page in 'Settings -> Deployments -> Pages' of your project.
