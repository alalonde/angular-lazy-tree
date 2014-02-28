angular-lazy-tree
=================

An AngularJS tree directive supporting lazily-loaded nodes

This features a recursive design where events are propagated up and down the tree nodes.  It requires an array defining the parent nodes, an attribute representing a node's ID, and a callback function to load children nodes.  This function can return a promise or an array of child nodes.

Other features:
* Auto-expand a given hierarchy of node IDs
* Auto-select a node.  Usually used in conjunction with auto-expansion.

Usage:
`angular.module('myApp', ['lazy-tree', ...]);`

Demo here: http://jsfiddle.net/alalonde/NZum5

More infomation here: http://blog.boxelderweb.com/2013/08/19/angularjs-a-lazily-loaded-recursive-tree-widget/

To Do: 
1. Extract some of the DOM-manipulation code into the template so it's easier to modify (e.g. the spinner image)
2. Improve event bubbling so that there is no need to broadcast events from an external controller for it to function correctly
3. Testing...