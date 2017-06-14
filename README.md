# /r/EthTrader Styles

This repository contains the CSS styles and associated image assets for the [/r/EthTrader](https://www.reddit.com/r/ethtrader) subreddit. Only moderators can update the subreddit styles, but pull requests from others are welcome.

## Getting Started

### Prerequisites

Because the styles exceed reddit's 100 KB file size limit on CSS, we use an NPM script to minify `styles.css`, stripping out unnecessary data like whitespace and comments. You will need to have Node.js installed on your machine to run this script.

1. [Install Node.js](https://nodejs.org/en/download/) if you don't have it already.
2. Clone this repository to your machine and navigate to it in your command-line interface.
3. Install the node modules for the project:

```
npm install
```
4. Install the `postcss` command line tool:

```
npm install postcss-cli --global
```

### Minifying the CSS

Once the prerequisites have been met, you can minify `styles.css` using the following command:

```
npm run build
```

This will output a new file, ```styles.min.css```, in the same directory. This file is intentionally ignored by git. Its contents can be pasted directly into the subreddit styles field on reddit.

## Deployment

 **Never** upload the CSS output directly to /r/ethtrader without testing it first. Always upload to a test subreddit first and verify that everything looks as expected at various screen sizes.