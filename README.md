# ami-viz
Interactive network visualisation of summarised output from [The Content Mine's](http://contentmine.org/) [AMI plug-in](https://github.com/ContentMine/ami-plugin).

![ami-viz screenshot](https://raw.githubusercontent.com/matthewgthomas/ami-viz/master/screenshot.png)

This implementation borrows heavily from [Jim Vallandingham's](https://twitter.com/vlandham) [Interactive Network Visualisation example](http://vallandingham.me/interactive_networks.html).

## Input files
Use [ami-summarise](https://github.com/matthewgthomas/ami-summarise) to create the JSON files `words.json`, `words_tdidf.json` and `species.json`, and put them in the `data` directory. I've included some sample files.

## Usage
Open `index.html`. It works best if you run a local web server: 

- either `thin start` (this repository contain a Gemfile and a config file for `thin`)
- or `python -m SimpleHTTPServer`

Blue nodes are keywords, species names etc. Orange nodes are articles. Hover over nodes for more info. Click article nodes to view the original paper. In case the networks are too big (for example if you have hundreds of articles), use your mouse's scroll wheel to zoom in/out. You can also drag the network around the screen.
