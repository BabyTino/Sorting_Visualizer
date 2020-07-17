# Sorting Visualiser using matplotlib in python

A Visualisation tool for sorting algorithms made using python's famous data visualisation library matplotlib.

![GIF](https://github.com/sharma-kunal/Sorting-Visualiser/blob/master/media/video_1.gif)

![GIF](https://github.com/sharma-kunal/Sorting-Visualiser/blob/master/media/video_2.gif)

## Installation

* Run the command

```
pip install matplotlib
```

to install matplotlib and it's all that you will need to run the visualiser.

## Running

* Go to the directory where you cloned the repo and just run the file `plot_graph.py` using the command

```
python plot_graph.py
```

And now you can choose the desired values after running the above command.

If you want to add more sorting algorithms, feel free to contribute to the project.

If you have any doubts or problems regarding the project, feel free to ask me.

## Explanation

Step 1: Instead of taking integers, I made every value an object with two attributes, color and value, so that I can change the color of every bar.

class Data:
	def __init__(self, value, color=None):
		self.value = value
		self.color = color if color else 'cyan' #default color is cyan

		Converting above arr to an object of above class

arr = [Data(i) for i in arr]
Now each element in this list has two attributes, value and color (default ‘cyan’).

Step 2: Now we create each frame describing each step of sorting with unique colors.

To understand the above line, let us sort a small list using Bubble Sort and divide it into steps.

arr = [12, 11, 13, 5, 6]

FRAME 1: arr = [Data(i) for i in arr]

Now each value has color ‘cyan’ in frame 1.


FRAME 2: We color arr[0] = ‘red’ and arr[1] = ‘black’


FRAME 3: We color arr[1] = ‘red’ and arr[2] = ‘black’


and so on.

Step 3: Now we have all the frames we want to plot. So we will use the matplotlib library to plot the frames one after another.

For that I used the Matplotlib’s Animation function. You can see how it’s working here

And the result looks something like


If you want to add more sorting algorithms, feel free to contribute to the project.