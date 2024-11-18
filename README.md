# authentikanban

## Description

The purpose of this app was to add JWT authentication to an existing Kanban board app, which is set up to be used as a web-development task tracker that can sort items into "todo," "in progress," and "done" catagories. 

To view tickets, the app requires users to login using valid, existing login info, which can be seeded into the database beforehand.

This app gave me practice implementing JWT authentication with a full-stack application, learn more about JWT's, and also deploying to Render while utilizing a postgres database.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

## Installation

Copy the SSH Key from the [GitHub Repository](https://github.com/dcartolano/authentikanban) and perform a git clone into a local directory of your choice. Open in VS Code or similar program. In the integrated terminal, run `npm i` to download all relevant node modules. 

Rename the `.env.EXAMPLE` file to `.env`. If you are using a local database, enter values for your database in the `DB_NAME`, `DB_USER`, and `DB_PASSWORD` fields. If you are using an online database provided by Render or a similar service, enter the provided external URL in the `DB_URL` field. For the `JWT_SECRET_KEY`, use any random string of your choosing.

Run the scripts `npm run build` followed by `npm run seed` to build the dist folders and seed the database.

## Usage

Provide instructions and examples for use. Include screenshots as needed.

To add a screenshot, create an `assets/images` folder in your repository and upload your screenshot to it. Then, using the relative filepath, add it to your README using the following syntax:

    ```md
    ![alt text](assets/images/screenshot.png)
    ```

If you only want to navigate to the deployed site, you can view it [here](https://authentikanban.onrender.com). To login, you must use one of the automatically seeded logins, which you can find in `server/src/seeds/user-seeds.ts` or see below. 

```js
    { username: 'JollyGuru', password: 'password' },
    { username: 'SunnyScribe', password: 'password' },
    { username: 'RadiantComet', password: 'password' },
```

If viewing locally, run the command `npm run start:dev` in the terminal. If the link does not open in a browser automatically, click or copy the link and open in your preferred browser.

## Credits

Thanks to EdX and Northwestern for the starter code and the opportunity to practice these skills. 

Thanks also to my instructor and the EdX tutors for all the help and clarifications along the way.

## License

n/a
