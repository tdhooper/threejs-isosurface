# THREE.IsosurfaceGeometry

three.js wrapper for https://github.com/mikolalysenko/isosurface

## Example

https://codepen.io/tdhooper/pen/QyEgYO

## Usage

```html
<script src="http://tdhooper.github.io/isosurface/build/isosurface.js"></script>
<script src="http://tdhooper.github.io/threejs-isosurface/IsosurfaceGeometry.js"></script>
```

```javascript

var d = 64;
var dims = [d, d, d];
var b = 1.5;
var bounds = [[-b, -b, -b ], [b, b, b]];
var map = function(p) {
  return p.length() - 1;
};
var geom = new THREE.IsosurfaceGeometry(dims, map, bounds);
var obj = new THREE.Mesh(geom, material);
scene.add(obj);

```
