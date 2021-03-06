# Harmonica and Boule: Modern Python tools for geophysical gravimetry

Leonardo Uieda<sup>1</sup>,
Santiago R. Soler<sup>2,3</sup>
Agustina Pesce<sup>2,3</sup>,
Lorenzo Perozzi<sup>4</sup>,
Mark A. Wieczorek<sup>5</sup>

> <sup>1</sup>Department of Earth, Ocean and Ecological Sciences, School of Environmental Sciences, University of Liverpool, UK
> <br>
> <sup>2</sup>CONICET, Argentina
> <br>
> <sup>3</sup>Instituto Geofı́sico Sismológico Volponi, UNSJ, Argentina
> <br>
> <sup>4</sup>Department of Earth Science, University of Geneva, Switzerland
> <br>
> <sup>5</sup>Laboratoire Lagrange, Université Côte d'Azur, Observatoire de la Côte d'Azur, CNRS, Nice, France

| | Information |
|---:|:----|
| doi | [10.5194/egusphere-egu21-8291](https://doi.org/10.5194/egusphere-egu21-8291) |
| Abstract | EGU21-8291 |
| Session | [G1.2: Mathematical methods for the analysis of potential field data and geodetic time series](https://meetingorganizer.copernicus.org/EGU21/session/39913) |
| When | Wednesday 28 April 2021 / 13:34 – 13:36 |
| Poster | [Download the vPICO poster (pdf)](https://github.com/fatiando/egu2021/raw/main/vpico.pdf) |

![vPICO poster for a quick 2-minute presentation of the abstract.](https://github.com/fatiando/egu2021/raw/main/vpico.jpg)

Gravimetry is a routine part of the geophysicists toolset, historically used in geophysics following the geodetic definitions of gravity anomalies and their related “reductions”.
Several authors have shown that the geodetic concept of a gravity anomaly does not align with goals of gravimetry in geophysics (the investigation of anomalous density distributions).
Much of this confusion likely stems from the lack of widely available tools for performing the corrections needed to arrive at a geophysically meaningful gravity disturbance.
For example, free-air corrections are completely unnecessary since analytical expressions for theoretical gravity at any point have existed for over a decade.
Since this is not easily done in a spreadsheet or short script, modern tools for processing and modelling gravity data for geophysics are needed.
These tools must be trustworthy (i.e., extensively tested) and designed with software development and geophysical best practices in mind.

We present the Python libraries Harmonica and Boule, which are part of the Fatiando a Terra project (https://www.fatiando.org).
Both tools are open-source under the permissive BSD license and are developed in the open by a community of geoscientists and programmers.

Harmonica provides tools for processing, forward modelling, and inversion of gravity and magnetic data.
The first release of Harmonica was focused on implementing methods for processing and interpolation with the equivalent source technique, as well as forward modelling with right-rectangular prisms, point sources, and tesseroids.
Current work is directed towards implementing a processing pipeline for gravity data, including topographic corrections in Cartesian and spherical coordinates, atmospheric corrections, and more.
The software is still in early stages of development and design and would benefit greatly from community involvement and feedback.

Boule implements reference ellipsoids (including oblate ellipsoids, spheres, and soon triaxial ellipsoids), conversions between ellipsoidal and geocentric spherical coordinates, and normal gravity calculations using analytical solutions for gravity fields at any point outside of the ellipsoid.
It includes ellipsoids for the Earth as well as other planetary bodies in the solar system, like Mars, the Moon, Venus, and Mercury.
This enables the calculation of gravity disturbances for Earth and planetary data without the need for free-air corrections.
Boule was created out of the shared needs of Harmonica, SHTools (https://github.com/SHTOOLS), and pygeoid (https://github.com/ioshchepkov/pygeoid) and is developed with input from developers of these projects.

We welcome participation from the wider geophysical community, irrespective of programming skill level and experience, and are actively searching for interested developers and users to get involved in shaping the future of these projects.

## Resources

Find out more:

* Harmonica documentation: https://www.fatiando.org/harmonica
* Boule documentation: https://www.fatiando.org/boule
* Tutorial for Boule and Harmonica at Transform 2021: https://youtu.be/0bxZcCAr6bw and https://github.com/fatiando/transform21

Get involved in the project:

* Join our Slack chatroom: http://contact.fatiando.org
* Come to an open community call: https://www.youtube.com/playlist?list=PLPA_RM8wsOqIEBLICo3v7f_A1WnLcwJld
* Follow Fatiando a Terra on Twitter: https://twitter.com/fatiandoaterra

## Citation

> Uieda, L., Soler, S. R., Pesce, A., Perozzi, L., and Wieczorek, M. A.:
> Harmonica and Boule: Modern Python tools for geophysical gravimetry,
> EGU General Assembly 2021, online, 19–30 Apr 2021, EGU21-8291,
> https://doi.org/10.5194/egusphere-egu21-8291, 2021.

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img
alt="Creative Commons License" style="border-width:0"
src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br>
This content is licensed under a <a rel="license"
href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution
4.0 International License</a>.
