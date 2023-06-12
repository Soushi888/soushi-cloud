# Soushi Cloud Frontend

This frontend is developed with Tauri, SvelteKit and TypeScript.
It use the Skeleton UI toolkit and Tailwind CSS.

## Specifications

- [ ] Connect to a Holochain conductor with websockets
- [ ] Display files and folders from a sync folder in the filesystem
- [ ] Sync the files and folders with the Holochain DHT
- [ ] Display a system tray icon
- [ ] Keep the app running in the background
- [ ] Send created, updated and deleted files to the Holochain DHT
- [ ] Receive created, updated and deleted files from the Holochain DHT

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:
pnpm add @tauri-apps/api
```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
