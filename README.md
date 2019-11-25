<h1>Offline Routing</h1>
<h3>Getting Started</h3>
<p>This project provides a way to route between points on a map, finding shortest and fastest routes. In addition, you
    can use it to solve Traveling Salesman Problem (TSP)</p>
<hr>


<h3>Prerequisites</h3>

<ul>
    <li>geojson file , eg. look up 'driving.geojson' file in the directory.</li>
    <li>Live server on visual studio code</li>
</ul>
<h3>Built With</h3>
<ul>
    <li><a href="https://nodejs.org/en//">NodeJs- Dependency Managemen</a></li>
    <li><a href="https://www.javascript.com/">Javascript - implementation language</a></li>
    <li><a href="https://visualstudio.microsoft.com/">Visual studio - The web framework used</a> </li>
</ul>
<hr>
<h3>Running the test</h3>
<ol>
    <li>copy the project </li>
    <li> replace 'driving.geojson' with our geojson file that represents the area tou want to work with.</li>
    <li>run the live streaming server on your visual studio.</li>
    <li>test py selecting the start and end points.</li>
    <li> a route will be presented to you.<insert pic>
    </li>
    <li>if you need the instructions press the 'instructions button'</li>
</ol>

<h3>Usage</h3>
Here is a list of the functions used in the algorithm, each one with the its usage.

<dl>
    <dt>build()</dt>
    <dd>taking the row network data from geojson file, it converts it to a graph[ nodes and edges]
        nodes being the intersections and edges is the route between those nodes represented each by a pk and required
        info ,eg. max speed, total distance and the substeps that build up the edge. resulting a graph that has an array
        of vertices.</dd>
    <dt>generateStepCoordinates()</dt>
    <dd> given the row data for the coordinates that represent the edge, it creates an array of object each has x,y
        proparities.</dd>
    <dt>drawroute()</dt>
    <dd>given a route( array of coordinates) it draws a polyline on the map</dd>
    <dt>function setInstructions()</dt>
    <dd> loops through the edges and finds the instruction needed to pass from edge to another depending on angel</dd>
    <dt>function distanceMatrix()</dt>
    <dd>given an array of coordinates, it builds a matrix of the distances between all the points.</dd>
    <dt>function tsp(matrix)</dt>
    <dd>given the distance matrix between nodes, it returns the shortest path to cross all those points
        .</dd>
    <dt>calculateDistance(v1, v2)</dt>
    <dd>given two points it reterns the distance between them in meters..</dd>
    <dt> function getMultiStepDistance(ss)</dt>
    <dd>given an array of coordiantes , it returns the total distance.</dd>
    <dt>toGeohash()</dt>
    <dd>given a point that is represented by its latitude and longitude, it returns the geohash code that represents
        this point</dd>
    <dt>route(source, destination)</dt>
    <dd>Given to vertices, it return an aray of the cordinates needed to be followed to reach from start point to end
        point.</dd>
    <dt>getLowestCost(Queue)</dt>
    <dd>given an array of points it returns the point with the lowest cost</dd>
