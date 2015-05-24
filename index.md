---
title       : Body Mass Index Calculator
subtitle    : A Shiny application
author      : John Cartmill
job         : Devloping Data Products Course
framework   : html5slides        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

####  Body Mass Index Calulator   
  
###### John Cartmill  
###### Developing Data Products  



--- .class #id 

## Why a Body Mass Index Calculator ?

Body Mass Index (BMI) is a good proxy for body fat percentage and has come to be widely used for preliminary diagnosis.

- More than one-third (34.9% or 78.6 million) of U.S. adults are obese.
- Obesity-related conditions include heart disease, stroke, type 2 diabetes and certain types of cancer, some of the leading causes of preventable death.  
- Obesity-related conditions include heart disease, stroke, type 2 diabetes and certain types of cancer, some of the leading causes of preventable death.  


Source US Center for Disease Control <br>http://www.cdc.gov/obesity/data/adult.html


--- .class #id 

## Simple and Easy to Use

The application only requires the user to move a slider bar for their height and weight and their BMI is instantly computed. Along with their BMI, a suggested weight loss goal is also calulated. 

The data is displayed in a table and the user's BMI is also plotted on a graph that shows BMI versus weight from a population taken from the National Health and Nutrition Examination Survey (NHANES).

--- .class #id 

## How it Works  

The formula for BMI is: Weight/Height^2  
Where weight is in kilograms and height is in meters. To "Americanize" the formula we convert Weight in pounds and and Height in inches to the appropriate units.    
Here is an example for 6 foot tall(72 inches), 180 pound person:

```r
Weight = 225/2.2
Height = 72/39.37
BMI = Weight/(Height^2)
round(BMI,2)
```

```
## [1] 30.58
```

--- .class #id 



## Sample Results  

Here is a sample of the ouput from the application.
<!-- html table generated in R 3.1.0 by xtable 1.7-4 package -->
<!-- Sun May 24 15:35:50 2015 -->
<table border=1>
<tr> <th>  </th> <th> Name </th> <th> Value </th>  </tr>
  <tr> <td align="right"> 1 </td> <td> Your Weight (lbs) </td> <td> 225 </td> </tr>
  <tr> <td align="right"> 2 </td> <td> Your Height(in) </td> <td> 72 </td> </tr>
  <tr> <td align="right"> 3 </td> <td> Your BMI </td> <td> 30.58 </td> </tr>
  <tr> <td align="right"> 4 </td> <td> Suggested Weight Loss </td> <td> 19 </td> </tr>
   </table>






