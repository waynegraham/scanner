# A Simple Accessability Scanner Wrapper

This is a simple wrapper for running [pall-ci](https://github.com/pa11y/pa11y-ci) on a set of web pages to generate an accessability report. 

## Installation

* Clone the repository
* Install the npm dependencies (`npm install`)
* Edit `package.json` and set the URL for the **sitemap.xml** to generate the report for.
* Run `npm run scan`

You can also just run:

`npx pa11y-ci --reporter=pa11y-ci-reporter-html --sitemap <path to sitemal>`

This will generate a report in `pa11y-ci-report`. You can open the file and see the errors.

## Settings

The `pa11y` config is set in `.pa11yci`. This follows the [pa11y configuration documentation](https://github.com/pa11y/pa11y#configuration). One setting that may be of use is setting the [runner](https://github.com/pa11y/pa11y#runners) and [concurrency](https://github.com/pa11y/pa11y-ci#default-configuration).

The settings in this are to use [axe-core](https://www.deque.com/axe/) and [htmlcs](https://squizlabs.github.io/HTML_CodeSniffer/).