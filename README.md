# Tailwind CSS Project Setup

This guide covers the steps required to set up and integrate Tailwind CSS into your project.

## Requirements

The following software is required for this project:

- **Node.js and npm**: Necessary to install and run Tailwind CSS.

### Installing Node.js and npm

To download Node.js and npm, visit the [Node.js official website](https://nodejs.org/) and download the version appropriate for your operating system. npm will be installed automatically during setup.

To verify that the installation was successful, you can run the following commands in your terminal:

    ```shell
    node -v
    npm -v
    ```

# Project Setup

## 1. Preparing the Project Directory

Navigate to the directory where you want to create your project and run the following command to initialize a Node.js project:

    ```shell
    npm init -y
    ```

## 2. Installing Tailwind CSS and Required Packages

To add Tailwind CSS and other necessary packages to your project, run the following command:

    ```shell
    npm install tailwindcss postcss postcss-cli autoprefixer
    ```

## 3. Creating Configuration Files

This command generates the `tailwind.config.js` file. Next, manually create a `postcss.config.js` file and add the following content:

    ```javascript
    module.exports = {
      plugins: {
        tailwindcss: {},
        autoprefixer: {},
      },
    }
    ```

## 4. Including Tailwind CSS in Your Project

Create a `src/main.css` file in your project directory and add the following Tailwind CSS directives:

    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

## 5. Building and Watching CSS Files

To build and watch the CSS file, run the following command in your terminal:

    ```shell
    npm run dev
    ```

## 6. Including CSS in Your HTML File

Create a `src/index.html` file and include the CSS file as follows:

    ```html
    <!DOCTYPE html>
    <html lang="en">
    
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Tailwind CSS Home Page</title>
        <link href="../dist/output.css" rel="stylesheet">
    </head>
    
    <body class="bg-gray-100 font-sans leading-normal tracking-normal">
        <!-- Content goes here -->
    </body>
    
    </html>
    ```

## 7. Start Developing Your Project

You have successfully integrated Tailwind CSS into your project. You can now begin developing your project by editing the `src/index.html` and `src/main.css` files.
