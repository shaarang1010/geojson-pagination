# geojson-pagination
Python and nodejs solutions for paginating large geojson file. 

## Motivation

Loading a large geojson file with >10000 points usually causes rendering and UX issues
on the UI.


## Proposed solution

Split the geojson files into managable points and paginate them according to the closet 
co-ordinates pased in the request body. 
Devs can specify the radius and get points closest to the users to begin with.

When the user expands the search radius, we can retrieve subsequest points by making 
additional api calls to specifying the page number
