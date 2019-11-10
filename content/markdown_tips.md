# List
## Unordered
* this
* that
    * here
    * there


## Ordered

1. item1
1. item2
1. item3
    1. item1.1
    1. item1.2
    1. item 1.3
    

## BlockQuotes
As Kanye West said:

> We're living the future so
> the present is our past.    



## Task List
### Very Importnat and Usefull
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item


## Tables
### Also very useful and important
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column



---
Below could be deleted
---
# Directory Structure

Aerobatic defaults to some specific common front-end conventions. By conforming to these conventions you can simplify your configuration (convention over configuration).

Here is the basic suggested skeleton for your app repo that each of the starter templates conforms to:

```bash
├── app
│   ├── css
│   │   ├── **/*.css
│   ├── favicon.ico
│   ├── images
│   ├── index.html
│   ├── js
│   │   ├── **/*.js
│   └── partials/template
├── dist (or build)
├── node_modules
├── bower_components (if using bower)
├── test
├── Gruntfile.js/gulpfile.js
├── README.md
├── package.json
├── bower.json (if using bower)
└── .gitignore
```

Your app's source code is nested beneath the `app` directory. This is where assets are served from in `debug` mode. Note that in most cases it is not necessary to setup a watch to re-compile languages and syntaxes including CoffeeScript, Sass, Stylus, Jade, and LESS as the development server will automatically do this for you in middleware. Note that in your index page, you should not include the `/app` prefix since the development asset server will treat it as the root.

```html
<!- Serves app/js/main.js-->
<script data-aero-build="debug" src="/js/main.js"></script>
```

For deployment, `yoke` assumes that all the files (including the index page) required to run in `release` mode have been written to a directory called either `dist` or `build` off the root. Grunt or Gulp both have good facilities for writing the outputs of a task to a different directory.
