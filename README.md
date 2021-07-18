# ReactJS - PWA (Progressive Web App) Boilerplate

> This is a ReactJS - PWA Boilerplate, created using `create-react-app`.

### Steps to Reproduce / Commands

- Create a PWA Enabled ReactJS App using the command:
  `npx create-react-app <YOUR APP NAME> --template cra-template-pwa`

- Navigate into the created folder/directory:
  `cd <YOUR APP NAME>`

- To run your app in the development mode:
  `npm start`

- Register a Service Worker

  > The directory of your newly created project contains the file `index.js`. Open it and find the following code:
  > Here, you can see that the serviceWorker is not registered yet. You have to change the `unregister()` call to `register()`.

- Configure the Web Application Manifest

  > Set up the web app manifest for your progressive web app that is located in the `manifest.json` file in public directory.

- Manifest attributes meaning:

  > - `short_name`: The name of your application, used within the icon, like on the users’ home screens or launchers.
  > - `name`: The name of your app shown in the app stores or browsers on startup screens and prompts. If `name` property is not defined, `short_name` will be displayed.
  > - `icons`: The set of icons (or just one), used on the users’ home screens, launchers, task switchers, splash screens, etc.
  > - `start_url`: The URL of the page of your app that your users see on the startup.
  > - `display`: This property is responsible for the browser view. The app can hide the address bar, run in the new window, go fullscreen, etc. See the attributes you can use for it:
  >   > - `fullscreen`: This option is for opening the app without any browser UI, occupying the entirety of the users’ display.
  >   > - `standalone`: This option allows for running the app in the new window, like a native app. It will also hide the browser UI elements like an address bar.
  >   > - `minimal-ui`: This option is quite similar to the previous one, but it comes with the minimal set of browser UI, like back and reload buttons.
  >   > - `browser`: This option enables the usual browser experience.
  > - `theme_color`: The color of the toolbar in your app.
  > - `background_color`: The color of the splash screen that appears when users click on the app icon in their home screens.​

- Install an npm package, `serve`
  `npm install -g serve`

- Run server and the app in Local
  `serve -s build`

- Make the App deployement ready
  `npm run build`

### To check performance, accessibility, and PWA compliance for your application

**`STEP 0`**: Install `Lighthouse` Chrome Extension, [Click here](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk?hl=en)
**`STEP 1`**: Open Chrome DevTools by choosing the **_Inspect_** option from the right-click menu on the page you need to inspect.
**`STEP 2`**: Go to the Lighthouse tab and click on the **_Generate Report_** button.
