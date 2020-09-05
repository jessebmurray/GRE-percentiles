# GRE-percentiles

ETS, which is the company that runs the GRE test, refuses to publish composite score data (verbal score + quantitative score). Instead, they only [publish the percentiles of the individual scores](https://www.ets.org/s/gre/pdf/gre_guide_table1a.pdf). 

ETS argues that the two primary multiple-choice tests they offer (separate from the Analytical Writing portion), are two different measurements that should not be combined. This is unlike the SAT, in which the Verbal and Mathematical portions are typically combined (through addition). In [ETS's words](https://www.ets.org/s/gre/pdf/background_and_technical_information.pdf): *"The GRE program recommends keeping the GRE Verbal Reasoning and Quantitative Reasoning scores separate when making admissions decisions and, therefore, does not provide a total score.*"


However, ETS made one fateful mistake. They [published the multiple linear regression equation relating the GMAT score and GRE scores](https://www.ets.org/s/gre/pdf/background_and_technical_information.pdf), which was measured from test-takers who *"took both the GRE General Test and the GMAT exam under actual operational, high-stakes conditions"*. 

This means that someone (like me) could use the multiple linear regression equation to obtain the GMAT score for each possible GRE score combination, and use the GMAT percentiles to obtain the GRE composite score percentiles. This is exactly what I've done through [this notebook](gre_percentiles-from_gmat.ipynb). It's worth noting that ETS does have a good point in that the same composite score can have a variety of GMAT percentiles, which is why I set the final percentile for each composite score to be equal to the median. To be thorough, I also provide the GMAT percentiles for all possible GRE scores. These are both in `csv`'s. 


|   Composite |   GMAT Percentile |
|------------:|------------------:|
|         260 |               0   |
|         261 |               0   |
|         262 |               0   |
|         263 |               0   |
|         264 |               0   |
|         265 |               0   |
|         266 |               0   |
|         267 |               0   |
|         268 |               0   |
|         269 |               0.5 |
|         270 |               0.5 |
|         271 |               0.5 |
|         272 |               1   |
|         273 |               1   |
|         274 |               1.5 |
|         275 |               1.5 |
|         276 |               2   |
|         277 |               2   |
|         278 |               2.5 |
|         279 |               2.5 |
|         280 |               3.5 |
|         281 |               3.5 |
|         282 |               4   |
|         283 |               4.5 |
|         284 |               5   |
|         285 |               5   |
|         286 |               6.5 |
|         287 |               7   |
|         288 |               7.5 |
|         289 |               8   |
|         290 |               9   |
|         291 |               9.5 |
|         292 |              10   |
|         293 |              12   |
|         294 |              12.5 |
|         295 |              13   |
|         296 |              14   |
|         297 |              15   |
|         298 |              16   |
|         299 |              18   |
|         300 |              19   |
|         301 |              21   |
|         302 |              23   |
|         303 |              24   |
|         304 |              26   |
|         305 |              28.5 |
|         306 |              30   |
|         307 |              31   |
|         308 |              35   |
|         309 |              36.5 |
|         310 |              39.5 |
|         311 |              41   |
|         312 |              44   |
|         313 |              47   |
|         314 |              49   |
|         315 |              52.5 |
|         316 |              56   |
|         317 |              58   |
|         318 |              63.5 |
|         319 |              66   |
|         320 |              67   |
|         321 |              73   |
|         322 |              75   |
|         323 |              78.5 |
|         324 |              81   |
|         325 |              82   |
|         326 |              85   |
|         327 |              88   |
|         328 |              89.5 |
|         329 |              92.5 |
|         330 |              95   |
|         331 |              96   |
|         332 |              97   |
|         333 |              97.5 |
|         334 |              98.5 |
|         335 |              99   |
|         336 |              99   |
|         337 |              99   |
|         338 |              99   |
|         339 |              99   |
|         340 |              99   |


