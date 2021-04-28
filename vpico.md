# Script for the vPICO 2 minute talk

For over two decades now, the geophysics gravimetry community has advocated
for the use of gravity disturbances in geophysics, instead of gravity
anomalies.

We believe that the availability of high-quality tools can help speed up the
adoption of these new ideas.

With that goal in mind, I would like to introduce the Python libraries: Boule
and Harmonica.

---

Boule provides representations of planetary ellipsoids and methods to calculate
normal gravity at any point.

This means that free-air corrections aren't needed for calculating gravity
disturbances with Boule.

In the bottom left you can see maps of the WGS84 normal gravity calculated with
Boule and the associated gravity disturbance.

Boule was born out of the shared necessity for this functionality in the
geophysics Python community, mainly SHTools and Harmonica.

It supports spheres and oblate ellipsoids and we're currently developing
tri-axial ellipsoids as well.

---

Harmonica is our library for dealing with potential field data.

It includes forward modelling, topographic correction, equivalent-source
methods, and more.

In the bottom right, you'll find an example of using Harmonica to calculate
residual Bouguer disturbances for the Bushveld Complex in South Africa.

We used prisms for topographic correction, removed a 2nd order trend, and
gridded to a constant height using equivalent-sources.

With Harmonica, we are trying to have an opinionated design of the code and
documentation to encourage the use of current best practices.

We are also developing new methods for equivalent-source processing, which you
can learn more about from Santiago's talk on Friday at session G4.3.

---

These projects are still evolving and we would like to invite this
community to get involved, whether it's coding, writing documentation, or
giving feedback.

You can do so by joining our Slack chat room, attending a community call, and
engaging with development on GitHub.

There are links for all of this in the abstract display materials and our
website fatiando.org

Thank you and we look forward to hearing from you!
