# Javascript

Operators
```javascript
// math
a % b // modulus
a *= b // a = a * b

// comparation
=== // equal value and equal type
== // equal
!= // not equals
! // NOT
```

Expressions
```javascript
typeof value // return type. Type and value 'undefined', means not assigned

( a == b ? value_if_true : value_if_else ) // conditional
```

Classes
```javascript
function Func(){
  var a = {};

  a.public_attrib = 1;
  a.public_method = function(){
    return 2;
  };

  return a;
}

or

function Func(){
}
function.prototype.public_static_method = function(){
  return 2;
};
function.prototype.public_static_attrib = 1;

// use
var an_object = new Func();
```

Threads
```javascript
var th = null;
th = setInterval( long_interval, function(){ /* logic here */ } );

// clear / reassign
clearInterval( th );
```

objects
```javascript
var an_object = { "attrib1": 1 };
an_object.attrib2 = 2;
an_object["attrib3"] = 3;
```

arrays
```javascript
// 1D array
var array_1d = [1, 2, 3];
// or
array_1d = [];
array_1d.push( 1 );
array_1d.push( 2 );
array_1d.push( 3 );

for( var i = 0; i < array_id1.length ; i++ ){ /* logic here */ }
// or
array_1d.forEach( function( item ){ /* logic here */ } )

// 2D array
var array_2d = [ [1, 2, 3]
               , [1, 2, 3] ];
var w = 3,
h = 2;
for( var i = 0; i < w ; i++ ){
  var column = array_2d[ i ];
  for( var j = 0; j < h ; j++ ){
    var cell = column[j]; // get

	// to set
    // column[j] = a_value;
  }
  // to set
  // array_2d[i] = column;
}

// filter array
var validation = function( item ){ /* return boolean value here */ };
var new_array = old_array.filter(validation);
```

Math
```javascript
// parse to int
parseInt( number );

// distance between ...
Math.sqrt( Math.pow(x1 - x2 , 2) + Math.pow( y1 - y2, 2 ) );

// random number between 0 and 1(?)
Math.random()

// radians to degrees
var degrees = radians * ( 180 / Math.PI );

// function: angle to [x, y]
return [ Math.cos( radians ) * magnitude, Math.sin( radians ) *  magnitude ];

// function: (x, y) to angle
var radians = Math.atan( x / y );
var degrees = radians * ( 180 / Math.PI );
return ( degrees < 0 ? 360 - degrees : degrees );
```