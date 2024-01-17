# Introduction to data visualization with matplotlib

- matplotlib have many interfaces, but we use object oriented intreface ( `pyplot`)
  - `import matplotlib.pyplot as plt` --> OOPs submodule importing
- `plt.subplots()` when called without any inputs creates 2 object. 
  - `figure` object 
  - `axis` object
  
- `figure` object is the container which holds everything that we see int he page. 
- `axis` is the part of the page that holds the data, It is the canvas on which we draw our data to visuilize it.
    
### Adding data to the axis

- We can add any number of data for different graphs
  - `ax.plot(X1_axis_data, Y1_axis_data)`
  - `ax.plot(X2_axis_data, Y2_axis_data)`
  - `ax.plot(X3_axis_data, Y3_axis_data)`

- To plot the figure in the canvas
  - `plt.show()`
  

### Customize the plot

- when we plot the figures the plot comes out to be continuous , but in reallity we gave it discrete data ploins. so to locate the dataploint in the figures we use `marker` argument
  - `ax.plot(X_axis_data, Y_axis_data, marker=MarkerType)`
  - Types of marker
    - "o" -> circle as marker
    - "v" -> pointing down triangles. etc... 
    - to get more markers check the documentation

- We can also change the apperiance of the connecting lines of the datapoints in the figures using `linestyle` argument.
  - `ax.plot(X_data, Y_data, linestyle=StyleType)`
  - Types of Style
    - "--"
    - None -> to remove the connector lines
- Elemenating the connector lines with `linestyle="None"`

- To change the color of the figure we use `color` argeument
  - `ax.plot(X_data, Y_data, color=ColorType)`
  - ColorType
    - "r" -> for red


### Customizing the axis labels

- naming the axis for clear visual understanding
- the axis object have many properties which is starts with `set` keyword, They are used to change certain propertie of the axis before ploting it.

- Giving X axis lable
  - `ax.set_xlabel("Labling the x axis name")`
- Giving y axis label
    - `ax.set_ylabel("labling the y axis name")`
- Giving titles to our axis
  - `ax.set_title("title name")`


### Small multiples

- when we have to add more data to plot lets say for example 10 datasets, and we plot all the data in single plot, it will become very messy, to understand the plots. So we use small multiple , it will create multiple plots in single axis(canvas), for different cases.
- In matplotlib small multiples is also called subplots , so thats why code is also used `subplot`

- Creating `rowNo` number of plot in row, and  `colNo` numer of plot in column
  - `fig, ax = plt.subplots(rowNo,colNo)`
  - Here fig and axis both have same index range from `[0 to rowNo-1][0 to colNo-1]` we use this notation to add data for different plots.
  - meaning to add data for 1st plot haveing index [0,0]. we use `ax[0,0].plot(X_data, Y_data)`

- there is special cases when we have created plots in single dimention, meaning it is only in row or column direction. for that case we only have to use one dimention to acess the plot 
  - `fig, ax = plt.subplot(2,1)`
  - ax[0] = plt.plot(X_data,Y_data)

- If we want to make all the plots have same range we can use a argument called `sharey`
  - `fig, ax = plt.subplots(rowNo,colNo, sharey=True)`
  - sharey is same as share y 
  

- TO give names to different plotted function in single figure, we use argument `legion`
  - `plt.legion("legion name)`

- To add grid all over the axis(canvas), we use `grid`
  - `plt.grid(True)`