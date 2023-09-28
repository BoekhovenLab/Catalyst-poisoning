# Catalyst-poisoning

We used the following set of ODEs to describe the systems by using a steady-state approximation that removed any explicit dependence on the concentration of O-acylurea and used an in house developed python model to fit the experimental data. 
The following set of ODEs was used and fitted. Ac stands for acid, F for fuel, W for waste, P for product and N for N-acylurea.
 
<img width="426" alt="image" src="https://github.com/BoekhovenLab/Catalyst-poisoning/assets/78074696/f6b43be1-3d00-4ab1-ab25-57bd44332cb2">


To fit the data, we used a homemade code inspired by previous works from Hartley’s group. The fitting procedure has been adapted from examples in the internet community, including https://tavoglc.medium.com/parameter-estimation-for-differential-equations-part-i-ordinary-differential-equations-443c6ba112ae.

Briefly, the code is meant to be run in a Google Collaboratory Jupyter Notebook to get the most out of the forms and interactive commands. However, it can also be downloaded and run it locally on your computer. 

The code is appropriately explained _in situ_. 

