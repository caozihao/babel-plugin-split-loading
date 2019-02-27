
# babel-plugin-split-loading [![NPM version](https://badge.fury.io/js/babel-plugin-split-loading.svg)](https://npmjs.org/package/babel-plugin-split-loading) [![Build Status](https://travis-ci.org/caozihao/babel-plugin-split-loading.svg?branch=master)](https://travis-ci.org/caozihao/babel-plugin-split-loading)

> 一个简易的babel插件，能自动拆分导入的依赖包，项目内有example，可供参考

##  example

```

import {flatten,join} from 'lodash'

<!-- 转换为 -->

import flatten from 'lodash/flatten';
import join from 'lodash/join';
```

## Installation

```sh
$ npm install --save babel-plugin-split-loading
```

## Usage

```.babelrc
  "plugins": [
    [
      "split-loading",
      {
        "library": "lodash",//你需要自动拆分的包名
      }
    ]
  ]
 
```

## License

MIT © [caozihao](https://github.com/caozihao)