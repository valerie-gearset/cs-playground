# gearset-website

### Getting started

- If node.js isn't already installed, install it: http://nodejs.org/download/
- Clone this repository
- Browse to the folder into which you've cloned the repo
- Run `npm install`

### Building + previewing the website

The build script will watch the source files (everything in `site/`) and generate built output (to `build/`) each time you save a change. To make the most of this:

- Browse to the root folder that you cloned the repository into
- Run `npm run watch`

Your local source of the website will now be built, and the output can be found in `build/`. To see the impact of your changes update in the browser:

- Go to http://localhost:3001/ in Chrome.
- Make some changes to the source!

### Build servers

Note that you can run a one-shot development build by just running `npm run dev`, or a production build by running `npm run prod`.

### Build failures

The website build also creates a sitemap for docs.gearset.com. This relies on an integration with the Intercom API (via the website API). If this fails, the entire build will also fail. In the event that this blocks the deployment of the website, the fetch in docsSitemap.js would need to be disabled. This may cause an empty sitemap to be submitted to Google, so take care when doing this. 
