# CS132 Group 7

## Initial Set-up

1. Clone repository through `gh repo clone ptrn23/cs132-group7`
2. Make sure you are in the right directory: `../cs132-group7`
3. Install dependencies through `pnpm install`
4. Run local webapp through `pnpm dev`
5. Open `localhost:5173` in browser. Yippee!!

# sv

Everything you need to build a Svelte project, powered by [`sv`](https://github.com/sveltejs/cli).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```sh
# create a new project
npx sv create my-app
```

To recreate this project with the same configuration:

```sh
# recreate this project
pnpm dlx sv@0.17.1 create --template minimal --types ts --add prettier eslint tailwindcss="plugins:none" --install pnpm ./
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```sh
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.
