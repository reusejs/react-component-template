<!-- [![View Storybook][view-storybook-image]][view-storybook-url] -->
[![Join Discord][join-discord-image]][join-discord-url]
[![NPM version][npm-version-image]][npm-url]
[![NPM downloads][npm-downloads-image]][npm-downloads-url]
[![MIT License][license-image]][license-url]
<!-- [![Storybook][storybook-action-image]][storybook-action-url] -->
[![NPM Publish][npm-publish-action-image]][npm-publish-action-url]

# React Component Template

This is a sample repository which can be used to develop new component libraries and push to NPM. Tailwind is integrated and purge is configured. So, when you make a final build, CSS would be send along with package.

### Where to write components?

1. There is a `src` folder where you can write your components
2. Whichever components you want to be exposed would go into: `index.js`

## Workflow

There are two ways you can develop components.

### Storybook

- Run: `yarn storybook` which will run the storybook in your localhost
- Open `src/Box/Box.stories.jsx` to find an example of Storybook
- When you write your own component, also write a `.stories.jsx` and storybook would pick it up

### Another ReactJS App

- Create a brand new react js app (Ex: my-app) using following: https://reactjs.org/docs/create-a-new-react-app.html#create-react-app
- Run `yarn link` in current component library. Ex: If you component name is react-component-template, you would run yarn link inside react-component-template
- Go to newly created reactjs app (my-app) and run `yarn link @reusejs/react-component-template`
- At the same time also run `yarn serve` in react-component-template, so that as you make changes, build happens simultaneously and your my-app refreshes it

## Contributing

### New components

Hit us on discord on `ideas` channel. Propose your ideas, we will blow our brains out.

### To existing components

Right now we don't a lot of hard and fast rules. 

Just follow: https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow

Basically:

- Fork the component to which you want to contribute
- Make your changes, test it properly
- Raise a Pull Request

## Releases

Once your pull request is made, a release would be schedule which will push the library to npm to @reusejs org. You can't push to reusejs org.
 
## License

react-component-template is freely distributable under the terms of the [MIT license][license-url].

[license-image]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat
[license-url]: LICENSE

[npm-url]: https://npmjs.org/package/@reusejs/react-component-template
[npm-version-image]: https://img.shields.io/npm/v/@reusejs/react-component-template.svg?style=flat

[npm-downloads-image]: https://img.shields.io/npm/dm/@reusejs/react-component-template.svg?style=flat
[npm-downloads-url]: https://npmcharts.com/compare/@reusejs/react-component-template?minimal=true

<!-- [view-storybook-image]: https://img.shields.io/badge/View-Storybook-F59E0B.svg
[view-storybook-url]: https://master--617258d6729860003a3d6e10.chromatic.com -->

[join-discord-image]: https://img.shields.io/badge/Join-Discord-7389D8.svg
[join-discord-url]: https://discord.gg/VUa9SHvvDb

<!-- [storybook-action-image]: https://github.com/reusejs/react-component-template/actions/workflows/chromatic.yml/badge.svg
[storybook-action-url]: https://github.com/reusejs/react-component-template/actions/workflows/chromatic.yml -->

[npm-publish-action-image]: https://github.com/reusejs/react-component-template/actions/workflows/publish.yml/badge.svg
[npm-publish-action-url]: https://github.com/reusejs/react-component-template/actions/workflows/publish.yml