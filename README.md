[Sublime Text Famo.us Snippets](https://github.com/pkiers/sublime-famous-snippets/)
========================================

A collection of [Famo.us](http://famo.us) code snippets for the [Sublime Text](http://sublimetext.com) editor.

## Installation
*1.*  Clone the repository into your packages folder.

    git clone git@github.com:pkiers/sublime-famous-snippets.git

*2.*  Download the [.zip](http://github.com/pkiers/sublime-famous-snippets/zipball/master) file and unzip it into your Sublime Text packages folder.

## Snippets

For now only the most used classes are added as snippets.

#### Require
    rc    var ... = require('...');
    rf    var ... = require('famous/...');

    re    var Engine = require('famous/core/Engine');
    rm    var Modifier = require('famous/core/Modifier');
    rr    var RenderNode = require('famous/core/RenderNode');
    rs    var Surface = require('famous/core/Surface');
    rt    var Transform = require('famous/core/Transform');
    rv    var View = require('famous/core/View');

    rms   var StateModifier = require('famous/modifiers/StateModifier');
    rsi   var ImageSurface = require('famous/surfaces/ImageSurface');
    rut   var Timer = require('famous/utilities/Timer');
    ruu   var Utility = require('famous/utilities/Utility');
    rvg   var GridLayout = require('famous/views/GridLayout');
    rvsc  var ScrollContainer = require('famous/views/ScrollContainer');
    rvs   var Scrollview = require('famous/views/Scrollview');

#### Instantiation
    ne    var {mainContext} = Engine.createContext();
    nm    var {modifier} = new Modifier({});
    nr    var {renderNode} = new RenderNode({});
    ns    var {surface} = new Surface({
              content: ''
          });
    nt    var {transform} = new Transform({});
    nv    var {view} = new View({}});

    nms   var {stateModifier} = new StateModifier({});
    nsi   var {imageSurface} = new ImageSurface({});
    nvg   var {gridLayout} = new GridLayout({
              dimensions: [1, 1]
          });
	nvsc  var {scrollContainer} = new ScrolLContainer({});
	nvs   var {scrollview} = new Scrollview({});

#### Miscellaneous
    sp    {mainContext}.setPerspective(1000);
    si    Timer.setInterval(function() {
              
          }, {1000});
    st    Timer.setTimeout(function() {
              
          }, {1000});

#### View
    view  /*globals define*/
          define(function(require, exports, module) {
               var View = require('famous/core/View');
               var Surface = require('famous/core/Surface');
               var Transform = require('famous/core/Transform');
               var StateModifier = require('famous/modifiers/StateModifier');

              /*
               * @name ${MyView}
               * @constructor
               * @description 
               */

              function ${MyView}() {
                  View.apply(this, arguments);
              }

              ${MyView}.prototype = Object.create(View.prototype);
              ${MyView}.prototype.constructor = ${MyView};

              ${MyView}.DEFAULT_OPTIONS = {
              };

              module.exports = ${MyView};
          });

## Author
Twitter: [pkiers](http://twitter.com/pkiers)
