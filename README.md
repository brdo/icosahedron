# icosahedron

#### Dependencies:

* numpy

#### Usage:
```bash
Usage: icosahedron.py [options]

Options:
  -h, --help     show this help message and exit
  --dual         Convert polyhedron to its dual
  --json         Display GeoJSON to stdout
  --level=LEVEL  Bifurcation level
```

#### Example:
```bash
python icosahedron.py --json --dual --level 3 > icosahedron.json && ogr2ogr -f PostgreSQL PG:"user=root password=secret" -overwrite -nln icosahedron icosahedron.json
```
