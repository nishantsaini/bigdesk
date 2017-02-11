# Bigdesk

Live charts and statistics for Elasticsearch cluster.

## Contents

- [Support Matrix](#support-matrix)
- [Release Notes](#release-notes)
- [Installation Instructions](#installation-instructions)
- [How to use Bigdesk](#how-to-use-bigdesk)
- [Supported Web Browsers](#supported-web-browsers)
- [Credits](#credits)

## Support Matrix

<table>
  <tr>
    <th>Bigdesk</th>
    <th>Elasticsearch</th>
  </tr>
  <tr>
    <td>master</td>
    <td>2.x.x</td>
  </tr>  
</table>

## Release Notes

#### Node status charts for es2.x (Feb 11, 2017)

- Fixes node stats charts and made them functional for elasticsearch 2.x
- Removed following charts: Process-CPU(%), File system (read-write charts)
- Added File system - file stores chart

#### Support for es2.x and cluster state support (Feb 1, 2017)

- Added support to install plugin with elasticsearch 2.x
- Fixed the cluster state chart

## Installation Instructions

Install Elasticsearch then navigate to `<ES_HOME>` and execute the following command on command line:

    $ ./bin/plugin install nishantsaini/bigdesk

## How to use Bigdesk

Once you open Bigdesk in your web browser, you need to **point it to the Elasticsearch node REST endpoint**.
For example if you run Elasticsearch locally the REST endpoint would be `http://localhost:9200/` by default.
You simply specify any endpoint URL in the text field on top of the Bigdesk screen (or via URL parameter, see below).

Now you should see cluster name and list of its nodes. You can switch between nodes in the cluster, new nodes are added
and old nodes are removed automatically on the fly.

You can change the Bigdesk **refresh interval** and **amount of data** that is displayed by charts.

## Supported Web Browsers

Bigdesk should work in all modern web browsers as long as they support SVG. It has been tested in Safari, Firefox and Chrome.

## Credits

Lukas Vlcek and [contributors](https://github.com/lukas-vlcek/bigdesk/contributors).

Modified by Nishant
