#  Common roles for data visualization include:

    - showing change over time
    - showing a part-to-whole composition
    - looking at how data is distributed
    - comparing values between groups
    - observing relationships between variables
    - looking at geographical data


### showing changes over time

- One of the most common applications for visualizing data is to see the change in value for a variable across time.
- These charts usually have time on the horizontal axis, moving from left to right, with the variable of interest’s values on the vertical axis


- There are multiple ways of encoding these values in plot.
  - Bar chart 
    -  encode value by the heights of bars from a baseline.
  - Line chart 
    -  encode value by the vertical positions of points connected by line segments. This is useful when a baseline is not meaningful, or if the number of bars would be overwhelming to plot.
  - box plot 
    -  can be useful when a distribution of values need to be plotted for each time period; each set of box and whiskers can show where the most common data values lie.
    -  used in statistics to display various parameters at glace
    -  median, interquartile range and outliers can be read easily
    -  data must be metric scaled
    -  schemetics of the plot
       -  dashed line is mean
       -  complete line is median
       -  rectangle upper side to rectangle lower side. is interquartile range, meaning they have 50% of the data .
       -  below 25% data found in rectange lower side 
       -  above 25% of the data found in rectangle upper side.
       -  maximum value without outliers is in between, upper T and lower T.... above and below T is outliers of the data.


### Charts for showing part-to-whole composition

- Sometimes, we need to know not just a total, but the components that comprise that total. While other charts like a standard bar chart can be used to compare the values of the components, the following charts put the part-to-whole decomposition at the forefront:
  - pie Chart
    - The pie chart and cousin donut chart represent the whole with a circle, divided by slices into parts
  - stacked bar chart 
    - A stacked bar chart modifies a bar chart by dividing each bar into multiple sub-bars, showing a part-to-whole composition within each primary bar.
  -  stacked area chart
     -  a stacked area chart modifies the line chart by using shading under the line to divide the total into sub-group values.


### Charts for looking at how data is distributed

- One important use for visualizations is to show how data points’ values are distributed. This is particularly useful during the exploration process, when trying to build an understanding of the properties of data features.

- Types of chart that can be used are :-
  - Bar Chart
    - Bar charts are used when a variable is qualitative and takes a number of discrete values.
  - histogram 
    - A histogram is used when a variable is quantitative, taking numeric values.
  - violin plot 
    - A violin plot compares numeric value distributions between groups by plotting a density curve for each group.
  -  box plot 
     -  The box plot is another way of comparing distributions between groups, but with a summary of statistics rather than an estimated distributional shape.
         

### Charts for comparing values between groups

- Another very common application for a data visualization is to compare values between distinct groups. This is frequently combined with other roles for data visualization, like showing change over time, or looking at how data is distributed.


- Types of chart that can be used are
  - Bar chart
    - A bar chart compares values between groups by assigning a bar to each group.
  -  dot plot
     -  A dot plot can be used similarly, except with value indicated by point positions instead of bar lengths. This is like a line chart with the line segments removed, eliminating the ‘connection’ between sequential points. Also like a line chart, a dot plot is useful when including a vertical baseline would not be meaningful.
  - line chart
    - A line chart can be used to compare values between groups across time by plotting one line per group.
  - scatter plot
    - The scatter plot is the standard way of showing the relationship between two variables.
  - bubl


### Charts for observing relationships between variables

- . The chart types below can be used to plot two or more variables against one another to observe trends and patterns between them.

- Types of chart used are
  - scatter plot
    - The scatter plot is the standard way of showing the relationship between two variables.
  - bubble plot
    - Scatter plots can also be expanded to additional variables by adding color, shape, or size to each point as indicators, as in a bubble chart.
  - connected scattered plot
    - When a third variable represents time, points in a scatter plot can be connected with line segments, generating a connected scatter plot.
  - duel-axis plot
    - Another alternative for a temporal third-variable is a dual-axis plot, such as plotting a line chart and bar chart with a shared horizontal axis.
  - heatmap
    - When one or both variables being compared are not numeric, a heatmap can show the relationship between groups. Heatmaps can also be used for purely numeric data, like in a 2-d histogram or 2-d density curve.

### Charts for looking at geographical data


- Sometimes, data includes geographical data like latitude and longitude or regions like country or state. While plotting this data might just be extending an existing visualization onto a map background (e.g. plotting points like in a scatter plot on top of a map), there are other chart types that take the mapping domain into account
- Two of these are highlighted below:
  - A choropleth is like a heatmap that colors in geopolitical regions rather than a strict grid.
  - Cartograms take a different approach by using the size of each region to encode value. This approach necessitates some distortion in shapes and topology.
