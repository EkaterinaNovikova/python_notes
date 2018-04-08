# Matplotlib

```import matplotlib.pyplot as plt```

### Line plot
Line plot which takes two lists as x and y arguments
```plt.plot(list1, list2)
plt.show()
```

### Scatter plot
``` plt.scatter(list1, list2)
plt.show()
```

### Histogram
```plt.hist(list, bins = 10)
plt.show()
```

### Customize plot

Logarithmic x-axis
```plt.xscale('log') ```

Labels for x and y axes
```
plt.xlabel()
plt.ylabel() 
```
Plot title
```plt.title()```

Ticks for x-axis
```tick_val = [1000,10000,100000]
tick_lab = ['1k','10k','100k']
plt.xticks(tick_val, tick_lab)```

