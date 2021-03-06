**Official Jokes App Remix Tutorial with atomic step-by-step commits**

- Current up-to-date [Official Jokes App Tutorial](https://remix.run/docs/en/v1/tutorials/jokes#jokes-app-tutorial)
- Nov 2021: Live Stream the whole 6-hour tutorial with Kent: [Remix Tutorial with Kent](https://www.youtube.com/watch?v=hsIWJpuxNj0)
  - Nov 2021: Original Github Repo [kentcdodds / remix-tutorial-walkthrough](https://github.com/kentcdodds/remix-tutorial-walkthrough)
- Atomic commits made for each tutorial section on my repo here as of May 9, 2022
- Any errors or omissions are my own

---

# Welcome to Remix!

- [Remix Docs](https://remix.run/docs)

## Development

From your terminal:

```sh
npm run dev
```

This starts your app in development mode, rebuilding assets on file changes.

## Deployment

First, build your app for production:

```sh
npm run build
```

Then run the app in production mode:

```sh
npm start
```

Now you'll need to pick a host to deploy it to.

### DIY

If you're familiar with deploying node applications, the built-in Remix app server is production-ready.

Make sure to deploy the output of `remix build`

- `build/`
- `public/build/`

### Using a Template

When you ran `npx create-remix@latest` there were a few choices for hosting. You can run that again to create a new project, then copy over your `app/` folder to the new project that's pre-configured for your target server.

```sh
cd ..
# create a new project, and pick a pre-configured host
npx create-remix@latest
cd my-new-remix-app
# remove the new project's app (not the old one!)
rm -rf app
# copy your app over
cp -R ../my-old-remix-app/app app
```
