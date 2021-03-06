# Getting Started

Welcome to Landr! Setting up Landr in your project is extremely easy. First,
make sure you install the `landr` CLI from npmjs.org if you haven't already by
running:

**Note:** _landr requires `libvips` or `vips`. Checkout the [installation here](https://libvips.github.io/libvips/install.html)_

```bash
npm install --global landr
```

Lets also install the excellent [`serve`](https://www.npmjs.com/package/serve)
static HTTP server as a way to preview our site:

```bash
npm install --global serve
```

Now that everything is in place, head over to your project's repository and
run:

```bash
landr build
```

Give it a bunch of seconds, and you should get various HTML, CSS, and
JavaScript files in the `dist` directory. You can preview your site by running:

```bash
serve dist
```

And pointing your browser to `localhost:5000`.

At this point, you have working, but not perfect, website. Landr generates
websites based on the content of the repository and relies on various OSS
conventions for doing its job. Making sure your repository is well structured
and follows the community conventions will do wonders for you website, and for
your repository overall!

Once you are happy with your site, run the following command to deploy to Netlify:

```bash
NETLIFY_AUTH_TOKEN=<token> landr deploy
```

Passing your Netlify authentication token as an environment variable.
