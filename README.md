# Admin

## Quick Start

```bash
git clone git@github.com:apeiro-tech/arsee_panel.git
cd arsse_panel
npm install
ng serve
```

`ng serve` should open a browser window to <http://localhost:4200>

By default angular runs on port 4200. To change this port you can run:

```bash
# This starts the development server on port 4205,
# but you can use any port you'd like
ng serve --port 4205  
``` 

## Generate Code
 
[Angular CLI](https://angular.io/cli/generate)
 

_Note: Creating a Component and a Container use the same command,
the difference is just the paths and how they are used._

### MVCC

Containers and Components are both Angular Components, but used in different ways.

Containers should arrange Components.

Obviously this can become subjective, but MVCC is the paradigm that we subscribe to.

## Troubleshooting

### npm start

If you receive memory issues adjust
`max_old_space_size` in the `ng` command of the `package.json`:

```json
"ng": "cross-env NODE_OPTIONS=--max_old_space_size=2048 ./node_modules/.bin/ng",
```

You can adjust 2048 to any number you need.

For more information about why you may need `--max_old_space_size`
see [this article](https://medium.com/@ashleydavis75/node-js-memory-limitations-30d3fe2664c0).
