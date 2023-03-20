# OM_4500x3528_C384_dev


## Development Documentation and Preliminary Analysis of Global 1/12 degree MOM6/SIS2/LM3 hindcast simulations

This is an initial simulation based on new ocean forcing protocols described in

Harrison et al, 2022 (https://doi.org/10.1029/2021MS002888)

The model is initialized from rest in 1982 using WOA05 hydrographic profile climatology for temperature and salinity (https://www.nodc.noaa.gov/OC5/WOA05/woa05data.html)

Model adjustment between the applied forcing and the prescribed initial conditions is an issue of concern. An important metric is the global ocean heat content (OHC), which should be relatively stable in a realistic scenario. The absence of surface salinity restoring (to a prior climatology) makes these simulation much more susceptible to catastrophic halocline collapse at high latitudes and subsequent cooling. This has been the experience using coarser resolution models, such as the 25km resolution OM4 simulation as described in Adcroft et al, 2019 (https://doi.org/10.1029/2019MS001726). Even in the presence of artificial sea-surface salinity (SSS) nudging, these simulation experience global cooling upon initialization fron near-present-day hydrographic observations. The present approach relies on realistic hydrologic forcing representation in order to maintain SSS. Global OHC is subject to initial cooling at coarse horizontal resolution in OM4. Simulations with the global 1/12 degree resolution model suggest that this rapid initial cooling is not an issue.



At eddy-resolving resolutions, as presented here, both mesoscale eddy representation is expected to exhibit more fidelity, in addition to reductions in spurious diapycnal mixing (https://doi.org/10.1016/j.ocemod.2011.10.003) .  Initial results suggest that high latitude maintenance of key circulation characteristics occurs at the present resolution. In particular, dense overflow properties are maintained downstream of key production regions in the Northwest Atlantic, and coastal Antarctica, where NADW and AABW watermass are known to originate.  Coarser resolution ocean models are deficient in this regard.

## The goal of the present effort is to provide a foundational model understanding for how key desne water forrmation and maintenance can be captured within a global context.

The initial 10 years of simulation are discarded due to potential spinup issues.  The primary focus of investigation is on the Atlantic thermohaline circulation and its fidelity with respect to in-situ moored observations obtained from colleagues at the Atlantic Oceanographic and Meteorological Laboratory (AOML).  Such observations are primarily of the deep component of the circulation below 2000m.  This lower limb of the AMOC is tied to dense water formation in the North Atlantic (NADW) flowing Southward, in opposition to Northward flowing denser watermasses formed around Antarctica (AABW).  Realistical formation rates, and maintenance downstream of watermass properties is critical for the maintenance of the circulation.  In addition, intermediate Sup-Polar watermasses  must be adequately represented.

These are exploratory simulations which bring together recent advancements in physically-plausible ocean hindcast forcing protocols, in addition to numerical advancements in ocean models with MOM6 and its quasi-Lagrangian finite-volume vertical coordinate formulation.

Pending publication, results are considered preliminary. In the interest of transparency, documentation is being made public for comment. Additional diagnostics can be made available upon request (Matthew.Harrison@noaa.gov)
