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

---

We have been developing these tools for only a few years and are still evolving
their goals and scope.

We want to invite this community to provide input and get involved in the
projects.

You can do so by joining our Slack chatroom, attending an open monthly
community call, and engaging with development on GitHub.

We are friendly and welcoming group with a range of different backgrounds.

There are links and more information about all of that on our website
www.fatiando.org.

There is also a link in the abstract display materials for further information,
including a recent tutorial and the code to generate the figures shown here.

Thank you and we look forward to hearing from you!
