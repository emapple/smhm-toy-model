# smhm-toy-model
A visualization of a toy model of the stellar mass-halo mass relation

In the notebook, you will find an interactive applet to see how different parameters of the stellar mass-halo mass (SMHM) relation affect both observational predictions and resulting inferences.

## Model description
The model assumes that the SMHM can be described by a broken power law with log-normal scatter. We have fixed the high-mass slope to the results of our [hydrodynamic simulations](LINK TO ARXIV). The low-mass slope (α), however, is allowed to vary. The scatter can also be adjusted, and is allowed to either be constant (σ) or growing (with slope γ). We assume every halo hosts a galaxy, but that there is some mass (m<sub>min</sub>) below which galaxies are unresolved, and therefore the halos are classified as "dark."

## Resolution-imposed biases

We also demonstrate the effects of resolution. First, we show the occupation fraction, which is the fraction of halos at a given mass that host a (resolved) galaxy. Since our underlying model assumes all halos host galaxies of some non-zero mass, an occupation fraction below 1 is a resolution effect. The location of the transition from 0 to 1 is subject to the slope of the SMHM and your resolution, and its width is determined by your scatter.

With scatter, limited resolution will lead to a survivorship bias in the remaining galaxies, such that they have higher stellar masses at a given halo mass. If not accounted for, this selection bias will lead to an _inferred_ SMHM slope that is shallower than the true underlying one. We show in the applet both the true underlying SMHM slope (which you can vary) and the naively inferred slope from the least squares regression on "observed" galaxies.

## Usage

To use the applet, clone or download the repository, and run the notebook. For example, from the command line:
```
cd
git clone https://github.com/emapple/smhm-toy-model.git
cd smhm-toy-model
jupyter notebook
```
and then from the browser, open `toy-model.ipynb` and run the notebook.

Only a few packages are required, but in case anyone wants I have also included a conda environment file.

## Contact

Please feel free to [email me](mailto:elaad.applebaum@gmail.com) with any questions or comments.
