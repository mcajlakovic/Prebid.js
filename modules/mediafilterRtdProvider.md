## Overview

**Module:** The Media Filter  
**Type: **Real Time Data Module  

As malvertising, scams, and controversial and offensive ad content proliferate across the digital media ecosystem, publishers need advanced controls to both shield audiences from malware attacks and ensure quality site experience. Media Filter, the market’s fastest and most comprehensive real-time ad quality tool, empowers publisher [Ad/Revenue Operations](https://mediatrust.com/who-we-help/adrevenue-operations/ "Ad/Revenue Operations") teams to block a wide range of malware, high-risk ad platforms, heavy ads, and ads with sensitive or objectionable content.

[![IMAGE ALT TEXT](http://img.youtube.com/vi/VBHRiirge7s/0.jpg)](http://www.youtube.com/watch?v=VBHRiirge7s "Publishers' Ultimate Avenger: Media Filter")

To start using this module, please contact [The Media Trust](https://mediatrust.com/how-we-help/media-filter/ "The Media Trust") to get a script and configuration hash for module configuration.

## Integration 

1. Build Prebid bundle with The Media Filter module included.  

```
gulp build --modules=mediafilterRtdProvider
```

2. Inlcude the bundled script in your application.

## Configuration

Add configuration entry to `realTimeData.dataProviders` for The Media Filter module.

```
pbjs.setConfig({
    realTimeData: {
        dataProviders: [{
            name: 'mediafilter',
            params: {
                configurationHash: '<configurationHash>',
            }
        }]
    }
});
```
