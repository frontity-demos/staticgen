---
title: Frontity
repo: frontity/frontity
homepage: https://frontity.org/
language:
  - JavaScript
license:
  - MIT
templates:
  - React
description: Create amazing websites using WordPress & React
twitter: frontity
---

**Frontity** is a free and open source framework to develop WordPress themes based on ReactJS. 

Frontity can be seen from two perspectives:

1. As an [alternative rendering engine for WordPress](https://docs.frontity.org/#an-alternative-rendering-engine-for-wordpress).
1. As a [React framework to create WordPress themes](https://docs.frontity.org/#a-react-framework-to-create-wordpress-themes).

---

## Install

Frontity has it's own CLI so you can just create a new Frontity project with a single command:

```text
npx frontity create my-app && cd my-app
```

This command will create a new directory with the following structure:

```text
my-app/
|__ node_modules/
|__ package.json
|__ frontity.settings.js
|__ favicon.ico
|__ packages/
    |__ mars-theme/
```

## Start development

Now you can start a development server with:

```text
npx frontity dev
```

This server will be listening to `http://localhost:3000` and watching for any changes inside the `packages` folder.

## Build

Once you are happy with your site and want to deploy it to production you can use

```text
npx frontity build
```

to create a production-ready bundle.

It will create a `/build` folder with a `server.js` file and a `/static` folder with all your javascript files and other assets. You can either

* Use `npx frontity serve` to run it like a normal Node app.
* Upload your `static` folder to a CDN and your server.js file to a `serverless` service, like [Now](../installation-and-deploy/deploy-on-now.md) or [Netlify](https://www.netlify.com/?ref=frontity).

----


Want to know more? 🧐 Check out [our docs](https://docs.frontity.org/getting-started)

Got questions or feedback? We'd love to hear from you. Come join our [community forum](https://community.frontity.org)! ❤️