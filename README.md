# TS scripts using Firebase Node Admin SDK

This is a template for creating and running admin scripts using the Firebase Node Admin SDK

Written with ES8, Typescript, and Node.js.

Use cases include emergency hotfixes and manual manipulations of your database (edits to your prod db should not be taken lightly)

--- 
## Get started

- Run `npm install` to install `firebase-admin`, `typescript`, etc.
- Add your dev/prod keys (e.g. ) to `/keys/`
    - Default path options:
        - `/keys/dev-service-account-key.json`
        - `/keys/prod-service-account-key.json`
    - If you use a different path instead of `/keys`, be sure to include it in `.gitignore` so you don't commit it to your VCS.
    - You can add more options or edit the name in `/src/index.ts`
    - By default, control flow for prod is commented out. Uncomment to enable

- Create your script in `src` 
    - Example: `/src/templateScript.ts`
    - Make sure to make the enclosed function the default export.

- Run it using `npm run script {env} scriptFilename`
    - Example: `npm run script dev templateScript` (if script is named `templateScript.ts`)
    - This compiles using `tsc` before running. See `package.json` for details.

--- 
### Other

Issues and Pull requests welcome!