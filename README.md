# Bibliophilia

![Bibliophilia](https://raw.githubusercontent.com/yuseiito/bibliophilia/master/logo.png)

## Requirements

- Node.js (Version is controlled by `.node-version`)
- npm

## Techinical Stack

This project uses the following technologies:

- 📖 [Remix docs](https://remix.run/docs)
- 📖 [Remix Cloudflare docs](https://remix.run/guides/vite#cloudflare)

## Development

Run the dev server:

```sh
npm run dev
```

To run Wrangler:

```sh
npm run build
npm run start
```

## DB migration

```sh
npx prisma migrate dev --name xxxx
```

## Typegen

Generate types for your Cloudflare bindings in `wrangler.toml`:

```sh
npm run typegen
```

You will need to rerun typegen whenever you make changes to `wrangler.toml`.

## Deployment

First, build your app for production:

```sh
npm run build
```

Then, deploy your app to Cloudflare Pages:

```sh
npm run deploy
```

## Styling

This application uses Radix UI for styling. You can find the documentation [here](https://www.radix-ui.com/docs/primitives/overview/introduction).
