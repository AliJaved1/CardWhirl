# sv

Everything you need to build a Svelte project, powered by [`sv`](https://github.com/sveltejs/cli).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npx sv create

# create a new project in my-app
npx sv create my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://svelte.dev/docs/kit/adapters) for your target environment.

# Requirements
- Users should be able to create/host a lobby 
- Users should be able to join an already created lobby (by entering a code or unique URL)
- Users should be able to play the game in real time with other users (e.g. via websockets)
- The host should be able to change game settings
- There should be multiple game modes that can be selected
i. Basic, where each card is worth 1 point, the team with the most points wins
ii. Cards have different values assigned to them (i.e. some cards are worth more points)
iii. Getting multiple cards correctly in a row can start a "combo" awarding extra points
- Users should be able to select "Correct" if they figure out the card's name
- Users should be able to select "skip" to skip the card
- Users should be able to shuffle the deck