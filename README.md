# GeoidApp--Things can be quite easier, and better

## What is GeoidApp

GeoidApp is a software application that can be used to compute various geoid components. Up to this moment it can efficiently compute the geoid height. We also intend to expand the features, you can also compute gravity anomaly and gravity disturbance, but they are still in beta. You can visit our website for further discussions about the GeoidApp features (GeoidApp)[https://geoidapp.github.io]

## About these results

We used several models in our evaluations. In particular we used `combined missions` egm2008, eigen-6c4, geco, and `satellite-only` mission ITU-GGC16, and ITU_GRACE16.

## The directory structure

A typical directory would contain:

- A directory _figure_ to store a plot of _std_ and _mean_ on it
- Three files
  - A log files which contains the std, and mean for particular model for each degree e.g. `The std for mode MODEL_NAME is: std_value, the mean is: mean_value for degree DEGREE`
  - csv file that contains `DEGREE, STD, MEAN`
  - A table which shows the best n-models (we use to output 10) based on the `std`

## EOF
LOL I don't have anything to mention, so yeah this is the end of the file. As if I need to tell Github that I'm done with them.
