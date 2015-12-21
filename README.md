# THREE.IsosurfaceGeometry

three.js wrapper for http://mikolalysenko.github.com/Isosurface/

## Usage

```html
<script src="http://tdhooper.github.io/isosurface/build/isosurface.js"></script>
<script src="http://tdhooper.github.io/three-isosurface/IsosurfaceGeometry.js"></script>
```

```javascript

var dims = [64,64,64];
var map = function(p) {
  return p.length() - 100;
};
var bounds = [[-11,-11,-11], [11,11,11]];
var geom = new THREE.IsosurfaceGeometry(dims, map, bounds);
var obj = new THREE.Mesh(geom, material);
scene.add(obj);

```
