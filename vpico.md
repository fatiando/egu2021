# Script for the vPICO 2 minute talk

> This is a guide for my 2 minute presentation.

Shifts in our practices as scientists happen slowly as ideas mature and gain
acceptance.

For example, several groups have advocated for the use of gravity disturbances
in geophysics, instead of gravity anomalies, for over two decades.

While there has been a lot of progress in this shift, adoption is still low
among non-specialists in gravimetry.

We believe that the availability of high-quality, tested, and well documented
tools can aid in the wider adoption of current best practices.

With that goal in mind, I would like to introduce two new Python libraries that
we have been developing for geophysical gravimetry: Boule and Harmonica.

---

Boule provides representations of planetary reference ellipsoids (like WGS84,
GRS80, Martian, and Lunar ellipsoids).

It also includes methods for coordinate conversion and calculating normal
gravity from these ellipsoids at any point outside of the masses using
analytical expressions.

This means that free-air corrections are a thing of the past and are no longer
needed for calculating gravity disturbances.

Boule was born out of the shared necessity for this functionality in the
geophysics Python community, mainly SHTools and Harmonica.

We originally had similar code in both projects and decided to create a
separate code-base that could be shared between projects with minimal
dependencies.

In the bottom left you can see a global map of the WGS84 normal gravity
calculated on the surface of the Earth using Boule and also the associated
gravity disturbance.

Boule supports spheres and oblate ellipsoids and we're currently developing
capabilities for tri-axial ellipsoids as well.

This last point is a testament to how community involvement can greatly benefit
a project, since I would never have thought to include spheres and tri-axial
ellipsoids because I don't encounter them in my own work.

---

Harmonica is our library for processing, modelling, and inversion of potential
field data.

At the moment, it includes forward modelling functions for prisms, tesseroids,
and point sources, topographic correction, equivalent-source methods for
interpolation and upward continuation, and more.

In the bottom right, you'll find an example of using Boule and Harmonica to
process gravity data from the Bushveld Complex in South Africa.

The final product is a grid of residual Bouguer disturbances calculated using
prisms for topographic correction, a 2nd order trend removal for
regional-residual separation, and gridding to a constant height using
equivalent-sources.

Many of our functions and classes are highly optimized using just-in-time
compilation and automatic parallelization where possible.

We are also developing new methods for equivalent-source processing that can
enable application to millions of data points without breaking your computer.

If you want to learn more about that, Santiago is giving a talk about it on
Friday at session G4.3.

With Harmonica, we are trying to have an opinionated design of the code and
documentation to encourage best practices in gravity and magnetics.

This means that we try not to set unreasonable defaults, encourage users to
understand the methods, and avoid adding functionality that should probably not
be used anymore (like free-air corrections).

---

We have been developing these tools for only a few years and are still evolving
their goals and scope.

We want to invite this community to get involved in the development, whether
it's coding, writing documentation, trying out new features, or giving
feedback.

You can do so by joining our Slack chat room, attending an open monthly
community call, and engaging with development on GitHub.

We are friendly and welcoming group with a range of different backgrounds.

There are links and more information about all of this on our website
www.fatiando.org.

There is also a link in the abstract display materials for further information,
including a recent tutorial and the code to generated all of the figures shown
here.

Thank you and we look forward to hearing from you!
