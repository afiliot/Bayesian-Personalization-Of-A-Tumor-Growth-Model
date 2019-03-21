# Bayesian-Personalization-of-a-Tumor-Growth-Model

In this project, we propose implement Lattice Boltzmann Method and Crank Nicholson scheme to simulate the growth of a particlarly infiltrative tumor : grade IV gliomas, also called glioblastomas mutliformes (GBM). This implementation is based on the article "MRI Based Bayesian Personalization of a Tumor Growth Model", from Lê et al. (2016). We use the MNI atlas to apply our growth model to real MRI (http://www.bic.mni.mcgill.ca/ServicesAtlases/ICBM152NLin2009). The equation under scrutiny is the so called FKPP (Fisher, Kolmogorov, Petrovsky, Piscounov) equation: 

<img src="http://www.sciweavers.org/tex2img.php?eq=%24%24%5Cfrac%7B%5Cpartial%20u%7D%7B%5Cpartial%20t%7D%20%3D%20%5Cnabla%28D.%5Cnabla%20u%29%20%2B%20%5Crho%20u%20%281-u%29%24%24&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0" align="center" border="0" alt="$$\frac{\partial u}{\partial t} = \nabla(D.\nabla u) + \rho u (1-u)$$" width="207" height="26" />

We use our simulations to recover the results from the Spherical Asymptotic Analysis from Harpold et al. (2007), "The evolution of mathematical modeling of glioma proliferation and invasion".

You can view our notebook on NbViewer for more convenience: 
https://nbviewer.jupyter.org/github/afiliot/Bayesian-Personalization-of-a-Tumor-Growth-Model/blob/master/Medical_Image_Analysis_Project_MVA.ipynb
