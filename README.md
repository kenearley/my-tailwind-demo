# My TailwindCSS Demo

I'm intrigued by TailwindCSS's [utility first approach](https://tailwindcss.com/docs/utility-first), but what sells me on this library is the [the ability to easily purge unused CSS](https://tailwindcss.com/docs/optimizing-for-production#writing-purgeable-html)

## Example

- run `yarn build` and the `./public/main.css` file is 324.14 KB
- run `yarn build:prod` and the `.public/main/css` fils is 4.05 KB

This is due to the fact that the plain html (`./public/index.html`) file is only using 3 utility classes. I just need to specify in the `tailwind.config.js` file which files to look at for purging. And it looks pretty simple to implement in any build system.

## To Run this demo

- `yarn`
- `yarn build` or `yarn build:prod`
- `yarn start`
