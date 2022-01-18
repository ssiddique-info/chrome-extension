# Simple chrome extension
Simple chrome extension that shows how to create a chrome extension from scratch.

This tutorial will show how to create a Google extension in any programming language. For demo purposes, we will be working with HTML and JavaScript. But chrome extensions can be created in any programming language.

## Step 1: Create the directory structure

We need to create a directory in which we will create the extension before we start writing code. For the extension to function properly, this directory must have a specific structure.

You will need 3 main components:

    description file
    icon
    HTML file


## Step 2: Create a description file

The description file is like a configuration file that Chrome needs to understand and correctly load the extension.

Here is an example of such a file `manifest.json` :

```
{
  "name": "Heppy Snowing",
  "description": "Simple Chrome extension shows snowflakes on Chrome screen",
  "version": "1.0",
  "manifest_version": 3,

  "permissions": ["activeTab", "scripting"],

  "action": {
    "default_popup": "popup.html",
    "default_icon": {
      "16": "/images/get_started16.png",
      "32": "/images/get_started32.png",
      "48": "/images/get_started48.png",
      "128": "/images/get_started128.png"
    }
  },

  "icons": {
    "16": "/images/get_started16.png",
    "32": "/images/get_started32.png",
    "48": "/images/get_started48.png",
    "128": "/images/get_started128.png"
  }
}

```

## Step 3: Create an extension system

This is where we write the functionality of your extension. It could be done in a variety of programming languages.

For simplicity, I have done it in HTML and JavaScript. We will be using the existing javascript framework that shows snow flakes on-screen and extends its functionality.

## Step 4: Front Extension for Chrome:

The HTML file contains the front end of the extension. It contains the button, that sits in the chrome extension position and displays a dropdown to enable the snow flakes on click action.

Step 5: Installing the extension on your local chrome to test


This is the most impressive move. We will publish our extension and see it in action.

For this you need:

    go to Chrome://extensions
    activate development mode;
    click unpacked;
    select a project;
    congratulations! Your extension has been loaded.
