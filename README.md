# 🚀 Static HTML Webpack Boilerplate
Based on - [Static HTML Webpack Boilerplate](https://github.com/erickzhao/static-html-webpack-boilerplate/releases).

## New features
- eslint
- webp images

## 🛠 Usage

- Available commands:
  - `npm run build`: Build files to the `dist` folder. Transpiles down to ES5 and bundles all JS into `app.bundle.js`. Transpiles SCSS to CSS and adds prefixing into `style.bundle.css`. Copies static assets and HTML over, and bundled CSS and JS gets added to HTML file.
  - `npm run start:dev`: Run `webpack-dev-server` at `localhost:9000`. Includes live reloading on any Javascript/SCSS/HTML changes.
  - `npm run start`: Builds files and runs a local production server on `localhost:8080` with `http-server`.
  - `npm run run lint:js`: Lints JS with ESLint.
  - `npm run lint:styles`: Lints SCSS stylesheets with stylelint.
  - `npm run lint:html`: Lints HTML for a11y issues using pa11y.
  
## 🔄 Continuous Integration

This boilerplate contains integration with [Travis CI](https://travis-ci.org/). The build system runs all linting scripts and deploys to GitHub pages upon push to the `master` branch. However, note that this deployment flow only works for Project Pages, as User and Organization pages [only support the master branch flow](https://help.github.com/articles/user-organization-and-project-pages/).

For more information on how to set up alternative deployment processes, check out the [Travis CI documentation on deployment](https://docs.travis-ci.com/user/deployment). The service can deploy to dozens of cloud providers, including Heroku, AWS, and Firebase.
