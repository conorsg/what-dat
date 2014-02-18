##NOLA Crime Stats Dashboard

Visualizations of data from [data.nola.gov](https://data.nola.gov/) made using [d3.js](http://d3js.org/)

###Notes

Use SoQL to transform raw data into:
 * counts of crimes by ZIP (http://data.nola.gov/resource/jsyu-nz5r.json?disposition=RTF&$select=zip,typetext,count(typetext)&$group=typetext,zip)

Build full dataset through paginated calls to get:
 * counts of crimes by type each week for last 52 weeks for big heatmap

##Problems

 * Cannot sort by day because of dumb timecreate format
 * Pulling all data by cycling through paginated data is resource intensive