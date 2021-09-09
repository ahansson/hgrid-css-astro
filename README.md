# Integrating [hgrid-css](https://github.com/ahansson/hgrid-css) in an [Astro](https://astro.build) project

<p>
  <img src="./assets/screenshot.png" alt="Screenshot" title="Screenshot">
</p>

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```
/
├── public/
│   ├── robots.txt
│   └── favicon.ico
├── src/
│   ├── components/
│   │   └── Tour.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

Install `hgrid-css` as a npm package with `npm i -D hgrid-css`. Change the file ending of `global.css` to `global.scss` and initialize hgrid at the top of the file: <pre><code>@use 'hgrid-css/sass/hgrid' with (
            <span class="text-gray inline-block push30h">// config (see https://hgrid.io/documentation/integrate for details)</span>
);</code></pre>

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command         | Action                                      |
|:----------------|:--------------------------------------------|
| `npm install`   | Installs dependencies                       |
| `npm run start` | Starts local dev server at `localhost:3000` |
| `npm run build` | Build your production site to `./dist/`     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://github.com/snowpackjs/astro) or jump into our [Discord server](https://astro.build/chat).
