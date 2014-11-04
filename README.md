find-free-port
--------

Find a free tcp port to listen locally.

## Installation

    npm install find-free-port

## Examples

Find a free port to listen on, begin from 3000

    var fp = require("find-free-port")
    fp(3000, function(err, freePort){
    });
    
Find a free port to listen on, begin from 3000, but stop at 3100 (not including 3100)

    var fp = require("find-free-port")
    fp(3000, 3100, function(err, freePort){
    });
    
Find a free port to listen on, begin from 3000, stop at 3100, bound to ip 127.0.0.1 only

    var fp = require("find-free-port")
    fp(3000, 3100, '127.0.0.1', function(err, freePort){
    });
    
