# md-article-template

A ready-made setup to write articles in Markdown and be able to see live preview and export the article in HTML

## Setup

You can [create your own GitHub repository from this template](https://help.github.com/en/articles/creating-a-repository-from-a-template) and have all the basic scaffolding under your control.

[![Use this template](https://img.shields.io/badge/GitHub-Use%20this%20template-blue)](https://github.com/lmammino/md-article-template/generate)

Once you created your own repo from this one, clone it locally and run `npm install` to get all the necessary dependencies for testing and building your Markdown article.


## Scripts

This template comes with some handy scripts to make editing markdown files a nicer experience:

### Test

 - `npm test`

With `npm test`, your `ARTICLE.md` will be tested for syntax errors using [`remark-lint`](https://npm.im/remark-lint).

### Live-Preview

 - `npm run preview`

With `npm run preview`, you will open an Electron window that will show a live preview of your `ARTICLE.md` and it will automatically update when you make changes to the source file. This command will be using [`vmd`](https://npm.im/vmd) under the hood.

### Build

 - `npm run build`
 - `npm run build:watch`

With `npm run build`, an HTMl version of the article will be created and named `ARTICLE.html`. This feature is built using [`generate-md`](https://npm.im/generate-md).

This command will also use `npm pack` to create an archive containing all the files related to the article so that you can easily share it with some third party.

If you wish to run the build every single time that your `ARTICLE.md` changes, you can do so by running `npm run build:watch`. This command will be using [`chokidar-cli`](https://npm.im/chokidar-cli) under the hood to watch for changes.


## Contributing

Everyone is very welcome to contribute to this project. You can contribute just by submitting bugs or
suggesting improvements by [opening an issue on GitHub](https://github.com/lmammino/md-article-template/issues) or [PRs](https://github.com/lmammino/md-article-template/pulls).


## License

Licensed under [MIT License](LICENSE). © Luciano Mammino.
