 [![Code of Conduct](https://img.shields.io/badge/%E2%9D%A4-code%20of%20conduct-blue.svg?style=flat)](https://github.com/edgi-govdata-archiving/overview/blob/main/CONDUCT.md)

# EDGI's Analysis of the Climate and Economic Justice Screening Tool (CEJST) Methodology
The Biden-Harris administration has long championed a "Justice40" approach to allocating climate-related spending. In early 2021, Biden signed Executive Order 14008, which directed government agencies to prioritize their investments in disadvantaged communities. To aid in this effort, the White House Environmental Justice Advisory Council (WHEJAC) met to make recommendations for determining what counts as a "disadvantaged community". In February 2022, the Council on Environmental Quality (CEQ) released its draft analysis for such a tool, drawing on similar approaches taken by US Environmental Protection Agency (EPA) in its EJScreen tool and the State of California's CalEnviroScreen.

EDGI generally supports the proposed methodology, and we believe it can deliver tangible benefits to communities. We conducted an independent analysis of CEJST, testing what it would look like to incorporate EPA datasets on government enforcement of and industry compliance with environmental protection laws like the Clean Air Act. Based on this analysis, we believe the methodology should consider:
- Growing the list of communities (Census tracts) based on the inclusion of additional criteria, namely, indicators related to enforcement and compliance. We find that an additional ~100 tracts could be identified as "disadvantaged" by including these indicators. 
- Evaluating what, at an economic structural level, unites the tracts already identified as disadvantaged. We find that a plurality of them are home to fossil-fuel electricity generating facilities, such as coal-fired power plants, and that many are also home to natural gas pipelines. As such, Justice40 should prioritize investing in community-level energy transitions, phasing out fossil fuel infrastructures that have disproportionately burdened low-income and racialized neighborhoods.
- Shrinking the list based on additional enforcement and compliance indicators. We find that ~1,000 out of the 23,000 tracts already identified (~5%) could be consider “priorities” based on limited enforcement of environmental protection laws and/or limited industry compliance with them.

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
