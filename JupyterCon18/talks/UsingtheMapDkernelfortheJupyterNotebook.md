# Using the MapD kernel for the Jupyter Notebook

## Randy Zwitch (MapD)

### in development to make python a first class citizen in mapd

### what is map d
* GPU accelerated SQL & Rendering Engine
* Server / GPU Based
  * MapD Core: SQL Engine
  * MapD Render: Vega Rendering Engine
  * Does the work to make a png and then push that to the browser
* Commercial product: Immerse
* github.com/mapd/pymapd
* MapD kernel for Jupyter

### examples
* DBI-compliant
* ibis: allows you to use pandas like code but take advantage of MapD acceleration
  * but really behind the scene it just turns your pandas into sql code
* jupyter specific functionality - %%mapd and then you're off to the races
