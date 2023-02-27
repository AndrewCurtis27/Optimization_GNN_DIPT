# Optimization_GNN_DIPT

# Running Instructions and Options

Download zip file. It contains .ipynb code file to be run, "dwpt_v5" folder with simulator network parameters, and empty "gp" folder for storing trained network parameters for later plotting and analysis. Open .ipynb file and run.

## Make sure the two following are present:
The subfolder "dwpt_v5" or its contents is present in your working directory, it has the weights for the simulator network. 

Subfolder in your working directory named "gp" is present, an empty one is included in the zip file, or create your own. This is to store the neural network model for later plotting. 

If using google colab, enable cuda. Go to runtime, change runtime type, select cuda. 

## Option instructions

n_noise is the number of noise "designs" sent to the generator and can be set at the neural network training loop code block. Default is 1000

n_epochs is the number of epochs of training for the neural network and can be set at the neural network training loop code block. Default is 500.

Loss function can be selected from listed options, this affects the training and distribution of the generator. Default is ProductofMeans.

p_set can be selected from listed options, this chooses which pairwise set will be chosen to show for highlighted plotting points.

points_to_plot is the number of points from the chosen p_set that will be highlighted and plotted. If this number is higher than the number of pareto points found, it will raise an error for the plot. Default is 1. 

save_figs is False by default, if set to True it will save the plots and diagrams
