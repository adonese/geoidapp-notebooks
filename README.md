# GeoidApp--Things can be quite easier, and better

## What is GeoidApp

GeoidApp is a software application that can be used to compute various geoid components. Up to this moment it can efficiently compute the geoid height. We also intend to expand the features, you can also compute gravity anomaly and gravity disturbance, but they are still in beta. You can visit our website for further discussions about the GeoidApp features [GeoidApp](https://geoidapp.github.io)

## About these results

We used several models in our evaluations. In particular we used `combined missions` egm2008, eigen-6c4, geco, and `satellite-only mission` ITU-GGC16, and ITU_GRACE16.

## The directory structure

A typical directory for any model would contain:

- A directory _figure_ to store a plot of _std_ and _mean_ on it
- Three files
  - A log files which contains the std, and mean for particular model for each degree e.g. `The std for mode MODEL_NAME is: std_value, the mean is: mean_value for degree DEGREE`
  - csv file that contains `DEGREE, STD, MEAN`
  - A table which shows the best n-models (we use to output 10) based on the `std`

## Figure

Is a directory to store our figures for combined models `std` results. Because of the difference between our models in degrees, we compared them on a `xlim` of 20 units up-to degree 180, then for the rest of the models (2190), we compared them with `xlim` of 100 units. We used a variable units for `ylim` to enhance the visualization. All of the figures were saved with _dpi_ of `1200` which is compatible with basically any journal.

You can view the figures [here](figures/)

There is also a \*.ipynb which is a jupyter notebook. We use it because it's a way better to visualize and work with your data than MATLAB/OCTAVE. This notebook might not be very clear, but I think I will get to document it better :)
For now, there are a few tables that contain some statistical results regarding the models i.e. what is the best degree over all models. Interestingly, we found that higher degrees have good results based on std (that shouldn't make any sort of surprise, but it's compared to Mohamed Osman's old results).

The figures are plots for the whole five models. It's also interesting to see that `egm2008, eigen-6c4, and geco` almost alwyas have the same std! It shouldn't be a surprise because I believe geco and eigen-6c4 shared some degrees from egm2008--I found that in their documentation if I remember.

## EOF
LOL! I don't have anything to mention, so yeah this is the end of the file. As if I need to tell Github that I'm done with them.
