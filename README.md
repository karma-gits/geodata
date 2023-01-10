# geodata / spider process
## 1. add names to where file
  1. open the where.data file
  2. add location/city/places... name on the list
  ### Example: i added 'Time Square' to the list

## 2. create a SQLlite table file from where.data
 * run geoload.py
 * in local folder> it will create a new 'geodata.sqlite' file (by removing old if exit).
 * with table column 'address' and 'geodata'
 * 'address' column will store all the names from the where.data file and 'geodata' will store thier geodatas
  ### Example: geodata.sqlite
  | address  | geodata |
| ------------- | ------------- |
| laguardia airport  | .....  |
| Time Square | .....  |
 

## 3. cleaning the datas from geodata.sqlite / create where.js file / create where.html file
   * run geodump.py to clean the lists
   * writes lat,lng, name on where.js file
   * writes where.html file to see tags on the map
   ### Example: 
    LaGuardia Airport (LGA), Queens, NY 11371, USA 40.7769271 -73.8739659
    Manhattan, NY 10036, USA 40.7579747 -73.9855426
  
## 4. open where.html to see the results
  ### Example: you can see the Times Square on the map.
  ![Image of Result](https://github.com/karma-gits/geodata/blob/1db9b5f50f8a32a5a2aaf875c550786ab45fbd83/3.result.png)
