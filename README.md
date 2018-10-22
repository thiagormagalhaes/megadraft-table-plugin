# WIP - Table Plugin - Megadraft Plugin
[![Build Status](https://secure.travis-ci.org/globocom/megadraft-table-plugin.png?branch=master)](https://travis-ci.org/globocom/megadraft-table-plugin) [![Dependencies](https://david-dm.org/globocom/megadraft-table-plugin/status.svg)](https://david-dm.org/globocom/megadraft-table-plugin) [![Dev Dependencies](https://david-dm.org/globocom/megadraft-table-plugin/dev-status.svg)](https://david-dm.org/globocom/megadraft-table-plugin?type=dev) [![Test Coverage](https://codeclimate.com/github/globocom/megadraft-table-plugin/badges/coverage.svg)](https://codeclimate.com/github/globocom/megadraft-table-plugin/coverage)

## Usage

Include the plugin in the `plugins` prop of your `Megadraft` instance.

```js
import React from "react";
import ReactDOM from "react-dom";
import {MegadraftEditor} from "megadraft";

import plugin from "megadraft-table-plugin";

class Example extends React.Component {
  render(){
    return (
      <MegadraftEditor plugins={[plugin]} />
    );
  }
}

ReactDOM.render(<Example />, document.getElementById("container"));
```

## Contributing

Install, run, test.

- Install npm dependencies
    make setup
- Gulp dev-server task with webpack + sass running on http://localhost:8080/
    make run
- Run mocha tests + eslint
    make test

If you're constantly running tests, there's a faster alternative using mocha's
watch feature:

```
make watch_unit
```

## Releasing

There's a `prepublish` script entry on `package.json` that runs build tasks
before publishing the package.

```
npm publish
```
