# firearms_analysis
An analysis of the trends in firearm background checks in America and its territories
### Introduction
On the 24th of May, 2022, an 18-year-old gunman shot and killed 21 people in an [elementary school in Texas](https://www.aljazeera.com/news/2022/5/25/texas-shooting-what-where-and-who). It is sad and horrible news and it raises the question of how that teenager was able to get access to a gun. It could be owned by someone he knows or by him, since he is of legal age. Either ways, it is, unfortunately, quite fitting to analyse information on background checks conducted for gun sales in America.
My analysis can be found in [this Jupyter notebook](https://github.com/ItunuoluwaOlowoye/firearms_analysis/blob/main/Investigating%20the%20FireArms%20Check%20Dataset.ipynb).

This dataset is from the FBI's National Instant Criminal Background Check System(NICS). It is used by gun shops to determine whether prospective buyers are eligible to buy firearms or not. 
**It is important to note that these numbers do not represent the number of firearms sold due to varying state laws and purchase scenarios.**

However, this dataset has generally been used as an acceptable proxy to determine firearm puchases.
The dataset contains background checks recorded from 1998 to 2017 in the different states in America. The month, state (including U.S. territories), and checks are recorded in columns. These include checks requested (column name in brackets):
* To issue a firearm permit or transfer (permit, permit_recheck, handgun, long_gun, other, multiple, admin)
* Before pledging or pawning a firearm (prepawn_handgun, prepawn_long_gun, prepawn_other)
* To regain possession of a firearm (redemption_handgun, redemption_long_gun, redemption_other)
* For returning firearms to previous owners (returned_handgun, returned_long_gun, returned_other)
* For loaning or renting a firearm (rentals_handgun, rentals_long_gun, rentals_other)
* To buy from or return a firearm to an unlicensed seller (private_sale_handgun, private_sale_long_gun, private_sale_other, return_to_seller_handgun, return_to_seller_long_gun, return_to_seller_other)
The total number of checks is also recorded in a column named 'totals'.

> Other refers to firearms that are not handguns or long guns. Multiple refers to a single background check for more than one type of firearm. Admin refers to administrative checks for other authorized uses of the NICS.

The full data description is found in the FBI file repository [here](https://www.fbi.gov/file-repository/nics_firearm_checks_-_month_year_by_state_type.pdf/view).

This dataset was supplemented with [population data from the 2016 U.S. census](https://www.google.com/url?q=https://d17h27t6h515a5.cloudfront.net/topher/2017/November/5a0a554c_u.s.-census-data/u.s.-census-data.csv&sa=D&source=editors&ust=1653921451986105&usg=AOvVaw1MavANZwewqQN29G-X61Ub) which contains the population of the U.S states (excluding U.S. territories) in 2016.
