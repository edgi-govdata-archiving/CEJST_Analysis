 [![Code of Conduct](https://img.shields.io/badge/%E2%9D%A4-code%20of%20conduct-blue.svg?style=flat)](https://github.com/edgi-govdata-archiving/overview/blob/main/CONDUCT.md)

# EDGI's Analysis of the Climate and Economic Justice Screening Tool (CEJST) Methodology
The Biden-Harris administration has championed a "Justice40" approach to allocating climate-related spending. In early 2021, Biden signed Executive Order 14008, which directed government agencies to prioritize their investments in disadvantaged communities. To aid in this effort, the White House Environmental Justice Advisory Council (WHEJAC) met to make recommendations for determining what counts as a disadvantaged community. In February 2022, the Council on Environmental Quality (CEQ) released its draft of such a tool, drawing on similar approaches taken by the US Environmental Protection Agency (EPA) in its EJScreen platform and the State of California's CalEnviroScreen.

We generally support the CEJST methodology, and believe it can deliver tangible benefits to communities. With that goal in mind, we believe CEQ should consider:

1. **Expanding the list of communities (Census tracts) based on the inclusion of additional criteria**, namely, indicators related to the enforcement of and compliance with environmental protection laws. We find that an additional 107 tracts could be added by including these indicators. 
2. **Evaluating what, in terms of economic forces, the tracts CEJST already identifies as disadvantaged have in common**. We find that a plurality of them are home to fossil-fuel electricity generating facilities, such as coal-fired power plants. Many are also home to natural gas pipeline facilities - the third most common facility type. CEJST should make it easy for the public to see these kinds of patterns and structures that operate across tracts, because they reveal drivers of “disadvantageness” rather than just outcomes. Doing so would also enable the public to see potential solutions - i.e. Justice40 should prioritize investing in community-level, community-led energy transitions, phasing out the fossil fuel infrastructures that have clearly burdened mostly low-income and racialized neighborhoods.
3. **Prioritizing the list based on additional enforcement and compliance indicators**. We find that 1,025 out of the 23,470 tracts already identified (4%) could be considered priorities based on limited enforcement of environmental protection laws and/or limited industry compliance with them.

You can run the analysis for yourself by running the two Jupyter Notebooks in this repo. We welcome any suggested edits or additions!

## Files
- `CEJST_prep.ipynb` pulls data from EDGI's copy of EPA data hosted by the Stony Brook University. It produces a single output file, `echo_data.csv`, that can be used as input for the analysis...
- `EDGI_CEJST_Analysis.ipynb` uses the output from `CEJST_prep.ipnyb` to extend the existing CEJST methodology with enforcement and compliance indicators of "disdvantageness." Inputs for this notebook also include the CEJST preliminary results themselves (drawn directly from the CEJST website), a list of industry classification codes (NAICS; drawn directly from its website), and Census data.
- `DECENNIALSF12010.P5_data_with_overlays_2022-03-30T170415.csv` is a US Census data file available [here](https://data.census.gov/cedsci/table?q=United%20States&t=Race%20and%20Ethnicity&g=0100000US%241400000&y=2010&d=DEC%20Summary%20File%201&tid=DECENNIALSF12010.P5).

---

## License & Copyright

Copyright (C) <year> Environmental Data and Governance Initiative (EDGI)
This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, version 3.0.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

See the [`LICENSE`](/LICENSE) file for details.
