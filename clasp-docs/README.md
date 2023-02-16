# The Clasp Tool

## Introduction

The Apps Script CLI, or `clasp`, is a tool that lets you to create, edit, and deploy [Apps Script](http://developers.google.com/apps-script/) projects locally. It allows you to create and publish web apps and add-ons for products like Sheets, Docs, Forms, and Slides from the command line. There are two ways you can develop Apps Script, using script.google.com or locally on your computer. We'll be learning the latter, how to use clasp, the command line tool for Apps Script.

## Features

- *Develop Locally*. `clasp` lets you write code on your own computer and upload it to Apps Script.
- You can also download existing Apps Script projects to your computer.
- Once the code is done,  you can use your favorite development tools like git to work on Apps Script projects.
- *Manage Deployment Versions*. Create, update and view multiple deployments of your project.
- *Structure Code*. `clasp` automatically converts your flat project on script.google.com into a structured project on your computer. For example,

```
# On script.google.com:
├── tests/slides.gs
└── tests/sheets.gs

# Locally:
├── tests/
│   ├─ slides.gs
│   └─ sheets.gs
```

## What you'll learn
This codelab will show you how to do 3 key activities with clasp:

- How to create new Apps Script projects
- How to clone, pull, and push existing projects
- How to manage deployments of your scripts

## Getting Started

### Downloading the CLI

The Apps Script CLI (clasp) requires Node.js >= v6.0.0 to be installed.
Once you have node, install the CLI globally (alias clasp):

```sh
npm i -g @google/clasp
```

### Login

Let's try out clasp! The only command you should remember is `clasp`.

```
clasp
```

This will show you the help menu for clasp. You'll see a list of commands and options. Let's login to your Google account.

```
clasp login
```

This will open a browser window and prompt you to login to your Google account. Once you login, you'll be given a code to enter into the terminal. Enter the code and you'll be logged in!

### Creating a New Project

Start out by creating a standalone Google Apps Script project with the following command:

```
mkdir clasp_codelab
cd clasp_codelab
clasp create --type standalone --title "Clasp Codelab"
```

This will create a new Apps Script project and download the code to your computer. You can see the code in the `clasp_codelab` directory.





