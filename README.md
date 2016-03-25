# aframe-site

> NOTE: The working docs have moved to https://github.com/aframevr/aframe/tree/master/docs

This site powers the __[A-Frame site](https://aframe.io/)__.

This site is built using [hexo](http://hexo.io/). Site content is written in [Markdown](http://daringfireball.net/projects/markdown/syntax) (and located in the [`src/`](src/) directory). Pull requests are welcome!


## Local Development

To install the dependencies and start the local development server:

    npm install && npm start

Then load __[`http://localhost:4000/`](http://localhost:4000/)__!

To clean the repo's local database:

    npm run clean

You may need to occasionally need to resart the server if you cause breaking changes. Just proceed as usual.


## Writing Documentation

First, make sure you have cloned the [core A-Frame library repo](https://github.com/aframevr/aframe).

    cd aframe
    npm link

And then have `aframe-site` point to that `aframe`:

    cd aframe-site
    npm link aframe

If you're curious, for the latest stable version of the docs, there's a soft link to the latest version of those directories in `src/docs` that points to `node_modules/aframe/docs/`. It was created like so:

    cd src/docs/
    ln -s ../../node_modules/aframe/docs/* .


## Deployment

To deploy this to production (GitHub Pages):

    npm run deploy

It will now be __[live](https://aframe.io/)__!


## Credits

Source adopted from the awesome [@vuejs](https://github.com/vuejs/) [site](https://github.com/vuejs/vuejs.org/).


## License

Licensed under [The MIT License](LICENSE).
