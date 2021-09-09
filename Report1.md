HW 1, CS 625, Fall 2021
================
Sara Negri
Sep 9, 2021

## Git, GitHub

1.  *What is your GitHub username?* SaraNegri94

2.  *What is the URL of your remote GitHub repo (created through
    Mr. Kennedy’s exercises)?*
    <https://github.com/SaraNegri94/myrepo.git>

## R

The command below will load the tidyverse package. If you have installed
R, RStudio, and the tidyverse package, it should display a list of
loaded packages and their versions.

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.4     ✓ dplyr   1.0.7
    ## ✓ tidyr   1.1.3     ✓ stringr 1.4.0
    ## ✓ readr   1.4.0     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

library(tidyverse)

## R Markdown

1.  *Create a bulleted list with at least 3 items*

CS 625

<ul>

<li>

Homework 1

</li>

<li>

Participation 2

</li>

<li>

Learning check

</li>

<li>

Midterm

</li>

2.  *Write a single paragraph that demonstrates the use of italics,
    bold, bold italics, code, and includes a link. The paragraph does
    not have to make sense.* install.packages(“rmarkdown”)

Hi everyone, I’m **Sara Negri**, an international student from Italy, of
<b><i> Master’s in Data science and Analytics </i></b>.

<p>

Today I will show you how **bold a text**.

<pre>
  <code>
   **put the text you want to bold**
  </code>
</pre>

<p>

Yesterday I created my first **e-portfolio** on Github, you can find it
<a href="https://saranegri94.github.io/saranegri.github.io/"> here</a>

3.  *Create a level 3 heading*
    <h3>
    It was my first time I worked with HTML language
    </h3>

## R

install.packages(“ggplot2”) mpg

#### Data Visualization Exercises

1.  (Q2) *How many rows are in mpg? How many columns?*

\#for rows

count(mpg)

\#or we can also do in this way

nrow(mpg)

\#for columns

ncol(mpg)

\#we have 234 rows and 11 columns

1.  (Q4) *Make a scatterplot of hwy vs cyl.*

x \<- mpg$hwy

y \<- mpg$cyl

plot(x, y, main=“HWY VS CYL”, xlab=“Hwy”, ylab=“Cyl”, pch= 20, frame=
FALSE)

![Alt text](/Users/saranegri/images/scatterplot.png)  
\#\#\#\# Workflow: basics Exercises

1.  (Q2) *Tweak each of the following R commands so that they run
    correctly (`library(tidyverse)` is correct):*

<!-- end list -->

``` r
library(tidyverse)
ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy))

filter(mpg, cyl == 8)

filter(mpg, displ > 3)
```

## Google Colab

1.  *What are the URLs of your Google Colab notebooks (both Python and
    R)?* Python:
    <https://colab.research.google.com/drive/1CjMQTJ_ycLqeX_PT9eqhgsJQebNVo-XI?usp=sharing>

r:
<https://colab.research.google.com/drive/1nJz0dN614vUyTfYmlKF240jb1893pJwF?usp=sharing>

## Tableau

*Insert your the image of your final bar chart here*
install.packages(“devtools”)
devtools::install\_github(“boxuancui/DataExplorer”, ref= “develop”)

![Alt text](/Users/saranegri/images/Sales_in_the_East.png)

1.  *What conclusions can you draw from the chart?*

From 2017 to 2020, the two categories, called bookcase and table,that
are characterized by negative profits or few profits. The table is the
least profitable category.

## Observable and Vega-Lite

### A Taste of Observable

1.  *In the “New York City weather forecast” section, try replacing
    `Forecast: detailedForecast` with `Forecast: shortForecast`. Then
    press the blue play button or use Shift-Return to run your change.
    What happens?* ![Alt text](/Users/saranegri/images/Newyork.png)
    \#there are less details about the weather

2.  *Under the scatterplot of temperature vs. name, try replacing
    `markCircle()` with `markSquare()`. Then press the blue play button
    or use Shift-Return to run your change. What happens? How about
    `markPoint()`?*

![Alt text](/Users/saranegri/images/scatterplot2.png)

\#the markpoint changed from a cicle shape to a square one

1.  *Under “Pick a location, see the weather forecast”, pick a location
    on the map. Where was the point you picked near?*

![Alt text](/Users/saranegri/images/map.png)

\#I choose a point that was in Longitute:-81.2 and latitude: 27.34 and
it was in Florida

1.  *The last visualization on this page is a “fancy” weather chart
    embedded from another notebook. Click on the 3 dots next to that
    chart and choose ‘Download PNG’. Insert the PNG into your report.*
    ![Alt text](/Users/saranegri/images/fancy.png)

### Charting with Vega-Lite

`markCircle()`

1.  *Pass an option of `{ size: 200 }` to `markCircle()`.* ![Alt
    text](/Users/saranegri/images/size200.png)

2.  *Try `markSquare` instead of `markCircle`.* ![Alt
    text](/Users/saranegri/images/square.png)

3.  *Try `markPoint({ shape: 'diamond' })`.*

`vl.x().fieldQ("Horsepower")`, … ![Alt
text](/Users/saranegri/images/diamond.png)

1.  *Change `Horsepower` to `Acceleration`* ![Alt
    text](/Users/saranegri/images/acceleration.png)

2.  *Swap what fields are displayed on the x- and y-axis*

![Alt text](/Users/saranegri/images/swap.png)

`vl.tooltip().fieldN("Name")` 1. *Change `Name` to `Origin`.* ![Alt
text](/Users/saranegri/images/origin.png)

Another example, `count()`

1.  *Remove the `vl.y().fieldN("Origin")` line.* ![Alt
    text](/Users/saranegri/images/noorigin.png)

2.  *Replace `count()` with `average("Miles_per_Gallon")`.* ![Alt
    text](/Users/saranegri/images/average.png)

## References

*Every report must list the references that you consulted while
completing the assignment. If you consulted a webpage, you must include
the URL.*

\*Reference 1, <https://rpubs.com/RatherBit/90926>

\*Reference 2,
<https://www.google.com/amp/s/www.wikihow.com/Create-Bold-and-Italicized-Text-in-HTML%3famp=1>

\*Reference 3, <https://www.w3schools.com/tags/tag_ul.asp>

\*Reference 4,
<https://r4ds.had.co.nz/data-visualisation.html#exercises>

\*Reference 5, <https://r4ds.had.co.nz/workflow-basics.html#exercises-7>

\*Reference 6, <https://r4ds.had.co.nz/data-visualisation.html>

\*Reference 7,
<https://www.earthdatascience.org/courses/earth-analytics/document-your-science/add-images-to-rmarkdown-report/>

\*Reference 8,
<https://observablehq.com/@observablehq/a-taste-of-observable>

\*Reference 9, <https://observablehq.com/@observablehq/vega-lite>

\*Reference 10,
<https://help.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-focus.htm>

\*Reference 11,
<https://observablehq.com/@observablehq/vega-lite-chart-types>

\*Reference 12, <https://rpubs.com/RatherBit/90926>
