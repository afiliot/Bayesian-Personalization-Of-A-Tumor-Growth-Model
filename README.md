# Bayesian-Personalization-of-a-Tumor-Growth-Model

In this project, we propose implement Lattice Boltzmann Method and Crank Nicholson scheme to simulate the growth of a particlarly infiltrative tumor : grade IV gliomas, also called glioblastomas mutliformes (GBM). This implementation is based on the article "MRI Based Bayesian Personalization of a Tumor Growth Model", from Lê et al. (2016). We use the MNI atlas to apply our growth model to real MRI (http://www.bic.mni.mcgill.ca/ServicesAtlases/ICBM152NLin2009). The equation under scrutiny is the so called FKPP (Fisher, Kolmogorov, Petrovsky, Piscounov) equation: $$\frac{\partial u}{\partial t} = \nabla(D.\nabla u) + \rho u (1-u)$$
with $$D\nabla u \cdot n_{\partial \Omega} = 0$$ which describes an anisotropic diffusion with a logistic proliferation term. 
$$D = d_w I_{3\times3}$$ in white matter and 
$$D = \frac{d_w}{10} I_{3\times3} = d_g I_{3\times3}$$  to account for the fact that it is clinically admitted that tumor cells have higher motility in white matter, compared to gray matter.

We use our simulations to recover the results from the Spherical Asymptotic Analysis from Harpold et al. (2007), "The evolution of mathematical modeling of glioma proliferation and invasion".

You can view our notebook on NbViewer for more convenience: 
https://nbviewer.jupyter.org/github/afiliot/Bayesian-Personalization-of-a-Tumor-Growth-Model/blob/master/Medical_Image_Analysis_Project_MVA.ipynb
