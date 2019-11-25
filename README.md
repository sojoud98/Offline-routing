<h1>Offline Routing</h1>
<p>This project provides a way to route between points on a map, finding shortest and fastest routes. In addition, you can use it to solve Traveling Salesman Problem (TSP)</p>
<hr>
<h3>Getting Started</h3>
<ul>
  
  </ul>
  <h3>Prerequisites</h3>
   <ul>
  <li>geojson file , eg. look up driving.geojson' file in the directory.</li>   
  <li>Live server on visual studio code</li>  
  </ul>
  <h3>Installing</h3>
  <h3>Running the tests</h3>
  <p>Run the live server of Visual Studio Code</p>
  <h3>Built With</h3>
     <ul>
  <li><a href= "https://www.javascript.com/">JavaScript</a></li>
  <li><a href="https://visualstudio.microsoft.com/" >Visual Studio Code</a> </li>  
  </ul>
<hr>
<h3>Built With</h3>
     <ul>
 <li> Visual studio - The web framework used</li>
<li>NodeJs- Dependency Management</li>
<li>Javascript - implementation language.</li>
 
  </ul>
  <h3>Usage</h3>
  
<dl>
    <dt>function build()</dt>
    <dd>taking the row network data from geojson file, it converts it to a graph[ nodes and edges]
nodes being the intersections and edges is the route between those nodes represented each by a pk and required info ,eg. max speed, total distance and the substeps that build up the edge. resulting a graph that has an array of vertices.</dd>
    <dt>function generateStepCoordinates(coords)</dt>
    <dd> given the row data for the coordinates that represent the edge, it creates an array of object each has x,y proparities.</dd>

 <dt>function drawroute(Route)</dt> <dd>given a route( array of coordinates) it draws a polyline on the map</dd>
 <dt>function setInstructions()</dt>
 <dd> loops through the edges and finds the instruction needed to pass from edge to another depending on angel</dd>
<dt>function distanceMatrix()</dt> <dd>given an array of coordinates, it builds a matrix of the distances between all the points.</dd>
 <dt>function tsp(matrix)</dt>
 <dd>given the distance matrix between nodes, it returns the shortest path to cross all those points 
.</dd>
<dt>function calculateDistance(v1, v2</dt>
    <dd>given two points it reterns the distance between them in meters..</dd>
    <dt> function getMultiStepDistance(ss)</dt>
        <dd>given an array of coordiantes , it returns the total distance.</dd>
            <dt>function toGeohash</dt>
                <dd>given a point that is represented by its latitude and longitude, it returns the geohash code that represents this point</dd>
                    <dt>function route(source, destination)</dt>
                        <dd>Given to vertices, it return an aray of the cordinates needed to be followed to reach from start point to end point.</dd>
                        <dt> function getLowestCost(Q) </dt>
                        <dd>given an array of points it returns the point with the lowest cost</dd>

</dl>
