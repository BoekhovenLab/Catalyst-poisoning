# Catalyst-poisoning

# Suppressing catalyst poisoning in the carbodiimide-fueled reaction cycle 

The published of the article can be found in [Chemical Science]([https://chemrxiv.org/engage/chemrxiv/article-details/64af0d6d6e1c4c986b487372](https://pubs.rsc.org/en/content/articlelanding/2023/SC/D3SC04281B))

## Authors

Xiaoyao Chen, Héctor Soria-Carrera, Oleksii Zozulia, and Job Boekhoven*

## Abstract:

In biology, cells regulate the function of molecules using catalytic reaction cycles that convert reagents with high chemical potential (fuel) to waste molecules. Inspired by biology, synthetic analogs of such chemical reaction cycles have been devised, and a widely used catalytic reaction cycle uses carboxylates as catalysts to accelerate the hydration of carbodiimides. The cycle is versatile and easy to use, so it is widely applied to regulate motors, pumps, self-assembly, and phase separation. However, the cycle suffers from side reactions, especially the formation of N-acylurea. In catalytic reaction cycles, side reactions are disastrous as they decrease the fuel’s efficiency and, more importantly, destroy the molecular machinery or assembling molecules. To put that in perspective, a side reaction that irreversibly converts as little as 1% of the fuel into a side product would mean less than 5% of the molecular machine left after 100 cycles. Therefore, this work tested how to suppress N-acylurea by screening precursor concentration, its structure, carbodiimide structure, additives, temperature, and pH. It turned out that the combination of low temperature, low pH, and 10% pyridine as a fraction of the fuel could significantly suppress the N-acylurea side product and keep the reaction cycle highly effective to regulate successful assembly. We anticipate that our work will provide guidelines for using carbodiimide-fueled reaction cycles to regulate molecular function about how to choose an optimal condition.

<img width="526" alt="image" src="https://github.com/BoekhovenLab/Catalyst-poisoning/assets/78074696/f1dbd741-c3a1-4216-bcc9-2fe537beae64">

## Code

We used the following set of ODEs to describe the systems by using a steady-state approximation that removed any explicit dependence on the concentration of O-acylurea and used an in-house developed Python workflow to fit the experimental data. 
The following set of ODEs was used and fitted. Ac stands for acid, F for fuel, W for waste, P for product, and N for N-acylurea.

<img width="526" alt="image" src="https://github.com/BoekhovenLab/Catalyst-poisoning/assets/78074696/f6b43be1-3d00-4ab1-ab25-57bd44332cb2">

We also calculate the yield of the anhydride as yield = $\frac {k4*∫[An]dt} {[F]_0}$
To fit the data, we used a homemade code inspired by previous works from [Hartley’s group](https://www.hartleygroup.org/). The fitting procedure has been adapted from examples in the internet [community](https://tavoglc.medium.com/parameter-estimation-for-differential-equations-part-i-ordinary-differential-equations-443c6ba112ae)

The code is meant to be run in a Google Collaboratory Jupyter Notebook to get the most out of the forms and interactive commands. However, it can also be downloaded and run it locally on your computer. 

The code is appropriately explained _in situ_. 
- Héctor Soria Carrera wrote the code
