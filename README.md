# Highcharts-More

The universal **highcharts-more** module. This module can be loaded as an ES6, AMD, CommonJS or global module, in NodeJS or in the browser. It works with most modern module loaders ([ES6](https://github.com/ModuleLoader/es6-module-loader), [RequireJS](https://github.com/requirejs/requirejs), [SystemJS](https://github.com/systemjs/systemjs)). This package is generated based on the [highcharts v4.2.5](https://github.com/highcharts/highcharts/releases/tag/v4.2.5) release.
> [highcharts-more](https://www.npmjs.com/package/highcharts-more-node) requires the [highcharts](https://www.npmjs.com/package/highcharts) module

### What is Highcharts?
[Highcharts JS](http://www.highcharts.com/) is a JavaScript charting library based on SVG, with fallbacks to VML and canvas for old browsers. To avoid bloating the Highcharts core library, the Highcharts team deploy new chart types and features in a separate file called [highcharts-more.js](https://github.com/highcharts/highcharts-dist/blob/master/highcharts-more.js). In short, highcharts-more is extra functionality on top of Highcharts without modifying it's core code. It also allows you to use some charts types which don't exist in the "original" highcharts such as bubble, range, gauge and pollar charts.


### Example Usage in Node using SystemJS and jspm
*Please note that there are several ways to use Highcharts. For general installation instructions, see [the docs](http://www.highcharts.com/docs/getting-started/installation).*

> **Tip:** importing [highcharts-more](https://www.npmjs.com/package/highcharts-more-node) using the **global** module format will suffice for most applications ([example below]()). 

First, install the [highcharts](https://www.npmjs.com/package/highcharts) and [highcharts-more](https://www.npmjs.com/package/highcharts-more-node) packages.
```bash
$ jspm install npm:highcharts
$ jspm install npm:highcharts-more-node   # or => jspm install github:clarketm/highcharts-more
```

Now import highcharts-more into your projects **after** the core highcharts module.
```js
// import Highcharts
import * as Highcharts from 'highcharts';

// import Highcharts-More
import 'highcharts-more'


export class GaugeChartExample {

  constructor() {
  
    // create the chart
    Highcharts.chart({
      chart: {
        type: 'gauge' // available ONLY with highcharts-more
      },
      // ...................................
      // ... chart configuration options ...
      // ...................................
    });
  };
  
}
```


##### Helpful links

* Official website:  [www.highcharts.com](http://www.highcharts.com)
* Download page: [www.highcharts.com/download](http://www.highcharts.com/download)
* Licensing: [www.highcharts.com/license](http://www.highcharts.com/license)
* Support: [www.highcharts.com/support](http://www.highcharts.com/support)
* Issues: [Working repo](https://github.com/highcharts/highcharts/issues)
