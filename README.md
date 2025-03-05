# 📚 LaTeX Template

This template repository provides a path to creating local LaTeX documents.

This requires an opinionated stack of tools, and as such, I have decided to use the following:

- VSCode: for its ability to have plugins and integration with GitHub and cruciallly, with its ability to use `Dev Containers` and work within a `Docker` container
- LaTeX Workshop: To build the document locally and provide autocompletion
- Error Lens: Highlights the errors from Grammarly and LaTeX build in the source code.
- Githubu Copilot to aid in writing latex and equations

# Workflow
To use this framework, follow these steps:

- Click on the green `Use this template` button and create your repository under your own GitHub. During this creation process, you can mark this as Private and thus only you can see your document
- Pull your GitHub repository locally.
- Open VSCode, make sure you have the `Dev Containers` from Microsoft extensions installed.
- Open the folder where you have cloned the repository. VSCode will prompt you to open this folder with the `Dev Containers` extension.
- Et Viola! You now have a working locally built, CI/CD integrated, LaTeX build. 

You can now:
- Modify `main.tex`. 
- Press `Ctrl+Alt+B` to initiate the shortcut for building the LaTeX file.
- You'll see a little spinning "Building" status bar indicator at the bottom
- Press `Ctrl+Alt+V` to see your newly Built PDF.

## Optionally:
- Commit your changes to GitHub once you've done some code. GitHub will then initiate the build PDF there as well.

## Optionally:
If you use [Overleaf](www.overleaf.com), you can link your overleaf account to your GitHub account and also collaborate there.
Pushing to the `main` branch from Overleaf will trigger the CI/CD GitHub Actions.


## Docker Image
The docker image, as seen in `.devcontainer/Dockerfile` uses Ubuntu 22.04 with the latest version of TeXLive-Full and thus should contain all the packages that a full tex installation would require

## GitHub Actions
I have specified a `.github/workflows` action that will build the PDF upon a push to the main branch. This wil trigger a build action and produce an Artifiact with the built PDF. 

Useful if you're using the GitHub Code editor (hint: press "." in GitHub).

## Contributing
If you would like to contribute, please fork/fix/pull requests as you see fit. I've provisionally placed the repository under an MIT license.
