# Axios Website

[![Netlify Status](https://api.netlify.com/api/v1/badges/8437c03b-f04a-4329-b619-3a82c0595f83/deploy-status)](https://app.netlify.com/sites/axios-docs/deploys)


The documentation page was built using [`inert static site generator`](https://github.com/codemaster138/inert). It works like this: inside the `docs` folder, there is a folder named `_src` (because GitHub automatically hides all files and folders starting with `_` from viewers on GitHub Pages). Inside this folder, there are some configuration, templates, styles, and, most importantly, in the `posts` folder, multiple markdown files containing the documentation.

To compile the documentation page, one must first install the inert CLI:

```bash
npm i -g inert-cli # yarn global add inert-cli
```

Now, open a terminal, navigate into the folder `docs/_src` and run the following command:

```bash
inert build
```

Inert will convert the markdown files into HTML, insert them into the templates, compile the `SCSS` styles and write the output into the `docs` directory.

This website was generously created by [@codemaster138](https://github.com/codemaster138)