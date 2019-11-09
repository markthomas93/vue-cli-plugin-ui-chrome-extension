# vue-cli-plugin-ui-chrome-extension

[![npm version](https://badge.fury.io/js/vue-cli-plugin-ui-chrome-extension.svg)](https://www.npmjs.com/package/vue-cli-plugin-ui-chrome-extension)

Start a chrome extension project with Vue-CLI UI (vue ui / vue ui -D) with ease!

<img src="./logo.png" height="48" width="48">

_Logo from FontAwesome_

## Installation

This plugin is meant for using new project for chrome extensions. Tested on default project of Vue, Vue with TypeScript

### For TypeScript

- Create a new project with `vue create test-project`, and select typescript without class-style component syntax
- Then, add this plugin with `vue add ui-chrome-extension`.

### For JavaScript

- Create a new project with `vue create test-project`.
- Then, add this plugin with `vue add ui-chrome-extension`.

### Run Development mode and Production

- Run development mode with `npm run build-watch` and a `dist` file will be generated. Install [Extension Reloader](https://chrome.google.com/webstore/detail/extensions-reloader/fimgfedafeadlieiabdeeaodndnlbhid) to reload chrome extensions easily everytime you reload. (take note that when u change manifest.json file, it will not automatically load, you need to remove and add the chrome extensions)
- Build for production `npm run build` and zip it and deploy onto chrome store.

## Current feature

- Generate manifest.json
- Generate popup.html
- Generate options.html
- Emit file out
- Support TypeScript (only generated with `vue add typescript`)

## Development

### Testing

#### Development

Currently, testing is done manually with the file `./auto.sh` / `./auto.bat`, by passing `-r` flag, it will delete the initial file generated.

#### Production

Test production code in npm as well with `./prod.sh` / `./prod.bat`.

### prompts.js

Vue CLI prompt is based on [inquirer.js](https://github.com/SBoudrias/Inquirer.js) api.

## Resources

- https://itnext.io/how-to-build-a-simple-vue-cli-plugin-a2e1323de1a0
- https://cli.vuejs.org/zh/dev-guide/plugin-dev.html

## Credit

- https://github.com/zwenza/vue-cli-plugin-build-watch
- https://github.com/RequireSun/vue-cli-plugin-chrome-extension
- https://github.com/sxei/chrome-plugin-demo
- https://github.com/superoo7/vue-cli-plugin-chrome-ext

## License

MIT
