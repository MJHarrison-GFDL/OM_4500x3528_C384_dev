# OM_4500x3528_C384_dev


## Development Documentation and Preliminary Analysis of Global 1/12 degree MOM6/SIS2/LM3 hindcast simulations

This is an initial simulation based on new ocean forcing protocols described in 

Harrison et al, 2022 (https://doi.org/10.1029/2021MS002888)

The model is initialized from rest in 1982 using WOA05 hydrographic profile climatology for temperature and salinity (https://www.nodc.noaa.gov/OC5/WOA05/woa05data.html)

Model adjustment between the applied forcing and the prescribed initial conditions is an issue of concern. An important metric is the global ocean heat content, which should be relatively stable in a realistic scenario. The absence of surface salinity restoring (to a prior climatology) makes these simulation much more susceptible to catastrophic halocline collapse at high latitudes. This has been the experience using coarser resolution models, such as the 25km resolution OM4 simulation as described in Adcroft et al, 2019 (https://doi.org/10.1029/2019MS001726). In these configurations, the initial roughly 20 years of the simulation are subject to significant drift from observations , due mainly to excessive ventilation in the Southern Ocean.  



At more eddy resolving resolutions, as presented here, both mesoscale eddy representation is expected to exhibit more fidelity, in addition to reductions in spurious diapycnal mixing (https://doi.org/10.1016/j.ocemod.2011.10.003) .  Initial results suggest that high latitude maintenance of key circulation characteristics occurs at the present resolution. In particular, dense overflow properties are maintained downstream of key production regions in the Northwest Atlantic, and coastal Antarctica, where NADW and AABW watermass are known to originate.  Coarser resolution ocean models are typically deficient in this regard, and the goal of the present effort is to provide a foundational model understanding for how these processes can be captured within a global context.

The initial 10 years of simulation are largely discarded due to potential spinup issues.  The primary focus of investigation is on the Atlantic thermohaline circulation and its fidelity with respect to in-situ moored observations obtained from colleagues at the Atlantic Oceanographic and Meteorological Laboratory (AOML).  Such observations are primarily of the deep component of the circulation below 2000m.  This lower limb of the AMOC is tied to dense water formation in the North Atlantic (NADW) flowing Southward, in opposition to Northward flowing denser watermasses formed around Antarctica (AABW).  Realistical formation rates, and maintenance downstream of watermass properties is critical for the maintenance of the circulation.  in addition, intermediate Sup-Polar watermasses which must be adequately represented.   

These are exploratory simulations which bring together recent advancements in ocean hindcast forcing protocols, which are more physically plausible, in addition to numerical advancements in ocean with MOM6 and its quasi-Lagrangian finite-volume vertical coordinate formulation.

Pending publication, results are considered preliminary. In the interest of transparency, documentation is being made public for comment. Additional diagnostics can be made available upon request (Matthew.Harrison@noaa.gov)


