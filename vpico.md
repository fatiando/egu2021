# Script for the vPICO 2 minute talk

> This is a guide for my 2 minute presentation.

Shifts in our practices as scientists happen slowly as ideas mature and gain
acceptance.

For example, several groups have advocated for the use of gravity disturbances
in geophysics, instead of gravity anomalies, for over two decades.

We believe that the availability of high-quality, tested, and well documented
tools can aid in the adoption of these current best practices.

With that goal in mind, I would like to introduce two new Python libraries for
geophysical gravimetry: Boule and Harmonica.

---

Boule provides representations of planetary reference ellipsoids and methods to
calculate normal gravity at any point.

This means that free-air corrections are not needed for calculating gravity
disturbances.

In the bottom left you can see a global map of the WGS84 normal gravity
calculated on the surface of the Earth using Boule and also the associated
gravity disturbance.

Boule was born out of the shared necessity for this functionality in the
geophysics Python community, mainly SHTools and Harmonica.

We originally had similar code in both projects and decided to create a
separate library that could be shared between projects.

It supports spheres and oblate ellipsoids and we're currently developing
capabilities for tri-axial ellipsoids as well.

---

Harmonica is our library for processing, modelling, and inversion of potential
field data.

It includes forward modelling, topographic correction, equivalent-source
methods, and more.

In the bottom right, you'll find an example of using Harmonica to calculate
residual Bouguer disturbances for the Bushveld Complex in South Africa.

We used prisms for topographic correction, removed a 2nd order trend, and
gridded to a constant height using equivalent-sources.

Many of our functions and classes are optimized using just-in-time
compilation and automatic parallelization where possible.

With Harmonica, we are trying to have an opinionated design of the code and
documentation to encourage the use of current best practices in gravity and
magnetics.

This means that we  avoid adding functionality that should probably not be used
anymore (like free-air corrections).

We are also developing new methods for equivalent-source processing, which you
can learn about from Santiago's talk on Friday at session G4.3.

---

We are still evolving the project goals and scope and would like to invite this
community to get involved, whether it's coding, writing documentation, or
giving feedback.

You can do so by joining our Slack chat room, attending an open monthly
community call, and engaging with development on GitHub.

There are links and more information about all of this in the abstract display
materials and our website fatiando.org

Thank you and we look forward to hearing from you!
