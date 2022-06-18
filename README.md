# eslint-config

My shared [ESLint](https://github.com/eslint/eslint) config.

## Overview

This repository contains ESLint configurations for the following setups:

- TypeScript with React

They are designed to be used together with [Prettier](https://github.com/prettier/prettier).

## Usage

1. **Install the required packages:**

   - TypeScript with React:

    ```sh
    npm i -D @webbergreg/eslint-config \
       @typescript-eslint/eslint-plugin \
       @typescript-eslint/parser \
       eslint \
       eslint-config-prettier \
       eslint-plugin-import \
       eslint-plugin-prefer-arrow \
       eslint-plugin-unused-imports
    ```

2. **Create the following entry in your `package.json` file:**

   - TypeScript with React:

    ```json
     {
     	"eslintConfig": {
     		"root": true,
     		"extends": ["@webbergreg/eslint-config/typescript-react"]
     	}
     }
     ```

3. **Add a linting script to your `package.json` file:**

   - TypeScript with React:

     ```json
     {
     	"scripts": {
            "lint": "npx eslint \"./src/**/*.*\"",
            "lint-fix": "npm run lint -- --fix",
     	}
     }
     ```