# Introduction
This article gives some examples of how using machine learning can affect the output of some stastical measurements. If unaccounted for, the use of ML algorithms may bias certain analysis, resulting in an apparently more precise measurement that is biased far away from the true result. The examples used are general, although inspired by cases found in High Energy Physics (e.g. particle classification). We'll use python and sklearn, although these affects are true for any ML. The code snippets below all form one script, a copy of which is in this github repo (tutorials folder), and begins with these imports:

```
import numpy as np
import sklearn
import matplotlib.pyplot as plt
```

# Setting the scene
Consider a typical classification problem involving two categories of event: ```A``` and ```B```. For each event, we're able to measure two features: ```x``` and ```y```. *We are trying to measure the shape of the distribution of ```x``` for category ```A``` events.*

> ## Real life example
> Say a Particle Physics experiment is interested in the energy spectrum of neutrinos. There are many types of signal that can minic a neutrino (i.e. a background), and reducing this background will increase the accuracy of the experiment. The energy spectrum of the background is typically lower than that of the neutrinos - energy it self is a useful descriminating parameter. But, as demonstrated below, using energy as a ML feature may bias the energy spectrum measured, if not accounted for correctly. 

As a demonstration, we'll randomly generate 1k events for the two categories based on some arbitrary typical distributions:

* Let A be distributed according to a 2D gaussian (i.e normal) distribution:
```
x_A = np.random.normal(1.0, 2, 1000) # Args are mean, RMS and num points.
y_A = np.random.normal(2.0, 1.0, 1000)
```
* Let B be distribute according to a exponential in ```x```, and uniform in ```y```:
```
x_B = np.random.exponential(1.0, 1000)
y_B = np.random.random(1000)
```
Lets first look at the data generated:
```
plt.scatter(x_A, y_A, label = 'A', size = 6)
plt.scatter(x_B, y_B, label = 'B', size = 6)
plt.xlabel('x')
plt.ylabel('y')
plt.show()
```
