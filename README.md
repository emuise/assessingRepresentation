
# Introduction

Protected areas (hereafter PA) are an integral component of biological conservation, designed to preserve ecosystem services and biodiversity both inside the PA and in some cases the surrounding regions [@chapeMeasuringExtentEffectiveness2005; @watsonPerformancePotentialProtected2014]. In recent decades, there has been a growing consensus of the need to conserve varying portions of the terrestrial area of the globe, with areal goals increasing over time [@cbd2010; @cbd2004]. In the 2010s, the Aichi biodiversity target sought to protect 17% of the entire globe [@cbd2010]. Nationwide, the Canadian government has set the goal of protecting 25% of Canada's terrestrial area by 2025 [@eccc2021]. While increasing proportional ecosystem protection does in turn aid conservation, it does not guarantee the representativeness of the entire ecosystem, nor that all biodiversity within the PA will be effectively conserved [@hazen2004].

Many conservation goals, both global and regional, are commonly based on the proportion of area protected, at least partly due to its ease of use and calculation [@brooks2004; @cbd2010]. However, while the area protected is a simple metric to report, other metrics can be more informative, with the potential to convey how effective a given PA is for protecting the inherent ecosystem services or biodiversity in the area [@chapeMeasuringExtentEffectiveness2005; @butchart2015; @maxwell2020]. Beyond areal extent, it is also relevant to consider the biases in PA placement, which are frequently located in fiscally cheaper, low productivity regions both globally [@venter2014; @joppa2009; @venter2018] and regionally, as is the case in British Columbia (BC), Canada [@environmentalreportingbc2016; @wang2020; @hamann2005]. The area metric heavily underestimates the global protected area required to adequately protect biodiversity, which research indicates is up to 50% of each ecoregion [@dinersteinEcoregionBasedApproachProtecting2017; @dinerstein2019].

In response to the proportion protected approach, a number of other methodologies have been developed to evaluate the effectiveness of PAs before these larger global targets have been met [@boltonUncoveringRegionalVariability2019; @hansenTrendsVitalSigns2018; @parrishAreWeConserving2003; @gastonEcologicalEffectivenessProtected2006; @gastonEcologicalPerformanceProtected2008]. One recently identified concept in Canadian park management is ecological integrity. Ecological integrity is defined as an ecosystem having the expected "living and non-living pieces for the region", and where ecological processes occur at the expected frequency and intensity for the region [@parkscanadaEcologicalIntegrity2019]. Many potential ecological integrity indicators have been examined to capture biodiversity related processes within PA [@hansenTrendsVitalSigns2018; @hansenMonitoringForestEcosystem2021]. These indicators can then be interpreted manually or automatically, most often through examining temporal trends within the PA or by comparing the indicators to areas in known healthy reference ecosystems [@woodleyMonitoringMeasuringEcosystem1993].

Frequently, comparisons between PA and unprotected areas (UA) have been drawn in order to assess PA performance and health [@defries2005]. This allows for the PA or PA network to be taken in context of surrounding and/or similar ecosystems [@wiens2009]. There are, however, challenges associated with comparing the effectiveness of a PA network directly with UA. It can be difficult to identify suitable UA for comparison due to the increased prevalence of human pressure in UA [@geldmannGloballevelAssessmentEffectiveness2019], and the bias for PA to be in areas that would not have faced increased human pressure due to their remoteness [@joppa2009].

@ferraroCounterfactualThinkingImpact2009 prescribes the use of the counterfactual - comparing what has happened post-PA implementation with what would have happened if the PA were not implemented. The counterfactual method has recently been adopted in the literature as a more accurate method for assessing protected area management effectiveness [@ribasGlobalComparativeAnalysis2020]. This method is frequently employed using matching methods to select UA which directly correspond to the PA being analyzed, often matching based on topography, climate, land cover, and other variables [@geldmannGloballevelAssessmentEffectiveness2019; @coadMeasuringImpactProtected2015; @eklundWhatConstitutesUseful2019]. Collecting field data across both the PA and its counterfactual UA can often be time-and-cost prohibitive. The increasing prevalence of freely available imagery has led to satellite remote sensing becoming an essential tool for PA monitoring [@nagendraRemoteSensingConservation2013].

The opening of the Landsat archive in 2008 [@wulderOpeningArchiveHow2012] has played a significant role in the use of satellite imagery in conservation monitoring [@nagendraParksWorkImpact2008; @turner2015]. The availability of 30-m spatial resolution data since 1984 allows for assessment of temporal trends in satellite derived indicators [@boltonUncoveringRegionalVariability2019; @nagendraRemoteSensingConservation2013; @hansenTrendsVitalSigns2018], while the global coverage allows for comparisons between similar and differing ecosystems [@nagendraParksWorkImpact2008; @wulderOpeningArchiveHow2012]. Leveraging free and open-source optical remote sensing data products has allowed users to increasingly undertake comparisons across an entire jurisdiction's PA network [@boltonUncoveringRegionalVariability2019; @fraserMonitoringLandCover2009; @soverelCharacterizingForestFragmentation2010; @pôças2011; @skidmore2021], comparing them to ecologically similar UA [@buchanan2018; @turner2015]. These comparisons allow for an assessment of the effectiveness of a given PA or the entire PA network at representing regional biodiversity trends [@boltonUncoveringRegionalVariability2019; @soverelCharacterizingForestFragmentation2010; @turner2015].

Optical remote sensing technologies have offered a key approach to deriving indicators [@boltonUncoveringRegionalVariability2019; @burkhardMappingEcosystemService2012; @fraserMonitoringLandCover2009; @nagendraParksWorkImpact2008; @soverelCharacterizingForestFragmentation2010; @pereira2013] and detecting key terrestrial processes [@turner2003] to assess PA effectiveness at conserving ecological integrity [@nagendra2001; @nagendraRemoteSensingConservation2013]. These indicators derived from remote sensing technologies can be categorized and monitored at broad spatial extents and across temporal scales. Commonly used indicators include land cover proportion [e.g., forest type, wetland, and unvegetated, @parmenterLandUseLand2003; @olthofUsingSatelliteRemote2006], tree species [@nagendra2001], habitat classification [@lucas2011; @mcdermid2005], spectral information [@gillespie2005; @feeley2005; @nagendra2010], spectral heterogeneity [@rocchini2010], and ecosystem structure [@cohen2004; @goetz2007; @pôças2011; @soverelCharacterizingForestFragmentation2010] and function [@skidmore2021]. Moreover, remote sensing technologies enable the monitoring of terrestrial processes, such as natural and anthropogenic disturbance regimes [@boltonUncoveringRegionalVariability2019; @hermosilla2015; @alsdorf2007; @kerr2003], alongside biogeochemical cycles [@myneni2001], vegetation productivity [@running2004], and vegetation dynamics [@zhang2003]. Diversity in forest structural attribute measurements, often derived from light detection and ranging (lidar) is also a strong indicator of biodiversity, providing habitat, influencing food quality, and mediating microclimates [@guo2017; @gao2014].

Lidar enables the accurate characterization of treed vegetation structure (e.g. canopy height, canopy cover, basal area) across forested areas by measuring the time it takes for an emitted pulse of light to return to the sensor [@lim2003]. While the natural variation in vertical and horizontal forest structure has been extensively explored using lidar, comparisons between PA and UA have been less frequently drawn using these methods when compared to optical remote sensing [@nagendraRemoteSensingConservation2013]. The lack of previous comparisons has likely been due to the frequently limited extents of lidar acquisitions, a problem which has recently been solved by generating wall-to-wall metrics. These wall-to-wall metrics can be created by combining lidar data with times series of Landsat data, generating forest structural attributes across large regions and even entire countries [@wulderLidarSamplingLargearea2012; @matasciThreeDecadesForest2018].

As Canada progresses towards the national goal of 25% of terrestrial area protected by 2025, there is a growing need to better understand how PA compare to UA with respect to location, ecological classifications, elevations, productivity, and forest structure. In this study, we (1) examine the hypothesis that BC's PA network is biased towards high-elevation, low-productivity regions of the province using free and open remote sensing data products, and (2) identify underrepresented forest structures in PA in the province. To accomplish this, we examined the bias in PA placement by comparing ecoregional PA coverage and land cover classes by elevation, and disturbances by latitude across protected and UA in BC. We examine representative forest structural attributes by comparing the distribution of key indicators by ecological zone to determine the differences between PA and UA to find the most and least similar represented forest structures throughout the network. We conclude by highlighting the usefulness of these globally available, high quality, consistent, and transferable datasets and methods for assessing PA effectiveness.

# Methods

## Study Area

The province of British Columbia, Canada, covers 94.4 million ha, of which approximately 64% is forested [@bcministryofforestsBritishColumbiaForests2003], and encapsulates a wide variety of biomes and ecosystems. This diversity of ecosystems is in part due to the large area as well as variations in topography and climate. The existing Biogeoclimatic Ecosystem Classification (BEC) system disaggregates BC ecosystems into zones [@pojarBiogeoclimaticEcosystemClassification1987]. The broadest classification delineates 16 zones, which are further broken down into subzones, variants, and phases based on microclimate, precipitation, and topography [@meidingerEcosystemsBritishColumbia1991; @pojarBiogeoclimaticEcosystemClassification1987]. As a result, BEC zones vary widely in size (ranging from 0.25 million ha to 17.5 million ha), and in number of subzones (from 1 to 43; see Table 1).

Both the BC [@bcparks2012] and Canada-wide [@governmentofcanada2019] PA mandates commit to conserving ecological integrity across the network. The PA network in BC is designed to serve both ecological conservation and human recreation aims [@bcparks2012] and consists of a network of PA and PA complexes (multiple nearby PA which share the same conservation goals), with large variations in size, ranging from 0.02 to 987,899 ha (@fig:study-area).

![Figure 1: Terrestrial British Columbia including BEC zones and the location of PA selected in this study.](figures/bec_map.png){#fig:study-area}

## Data

### Biogeoclimatic Ecosystem Classification and Protected Areas

Boundaries for BEC zones and subzones were acquired using the **bcmaps** R package [@R-bcmaps]. Two BEC subzones were entirely subsumed by PA (Boreal White and Black Spruce - Very Wet Cool and Spruce -- Willow -- Birch - Very Wet Cool Shrub), whereas the Sub-Boreal Pine -- Spruce - Moist Cool subzone has no PA representation.

Boundaries for all PA in BC were obtained from the Canadian Protected and Conserved Areas Database (available from <https://cws-scf.ca/CPCAD-BDCAPC_Dec2020.gdb.zip>), current as of December 2020, and includes the International Union for Conservation of Nature (IUCN) classification for each PA. PA were selected for analysis following the criteria outlined in @boltonUncoveringRegionalVariability2019. Only parks which belonged to IUCN classes Ia, Ib, II, and IV were selected, as these categories are considered strictly protected. Protected areas \< 100 ha in size were also excluded from the analysis, as these mainly occurred in urbanized areas. After selection, 745 suitable parks managed under various jurisdictions (provincial, federal, NGOs), comprising 15.4% of the total terrestrial area of British Columbia, were studied [@environmentalreportingbc2016]. An equal sample of pixels equal to the area of PA or UA - whichever was lower - was randomly selected from both PA and UA for each BEC subzone. This sampling regime accounts for bias in topography, climate, and climax species due to the methods used to delineate BEC zones and subzones [@pojarBiogeoclimaticEcosystemClassification1987].

### Digital Elevation Model

The Advanced Spaceborne Thermal Emission and Reflection Radiometer (ASTER) digital elevation model (GDEM V2, 30 m) was used to examine biases in protected area land cover and ecological classification by elevation [@tachikawa2011].

### Landsat derived datasets

Land cover, forest disturbances, and forest structural attributes for BC were derived from the annual Landsat best-available-pixel (BAP) composites from 1984 to 2019 at 30-m spatial resolution generated using the Composite2Change (C2C) approach [@hermosillaMassDataProcessing2016]. These composites are generated by annually selecting the optimal observations, free from atmospheric effects (haze, clouds, cloud shadows), for each pixel from the catalog of available Landsat-5 Thematic Mapper (TM), Landsat-7 Enhanced Thematic Mapper Plus (ETM+), and Landsat-8 Operational Land Imager (OLI) imagery acquired during Canada's growing season using the scoring functions defined in @whitePixelBasedImageCompositing2014. The annual BAP composites are further refined by applying a spectral trend analysis over the Normalized Burn Ratio (NBR) at pixel level in order to remove unscreened noise, detect changes and fill data gaps with temporally-interpolated values, resulting in annual, gap-free, surface-reflectance image composites [@hermosilla2015]. During this process, forest disturbances are detected, characterized and attributed to a disturbance agent (i.e., wildfire, harvest, non-stand replacing disturbances) using a Random Forests classification model via the object-based analysis approach [@hermosillaIntegratedLandsatTime2015] with an overall accuracy of 92% ±2% [@hermosillaMassDataProcessing2016].

Annual land cover information for Canada was produced using the BAP composites following the Virtual Land Cover Engine framework [@hermosillaDisturbanceInformedAnnualLand2018]. This framework integrates post-classification probabilities, forest disturbance information and forest successional knowledge with a Hidden Markov Model to ensure logical land cover transitions between years. The classification comprises 12 land cover classes organized as either non-vegetated or vegetated. Non-vegetated classes included water, snow/ice, rock/rubble, and exposed/barren land. Vegetated land cover classes discriminated among non-treed and treed vegetation (land-cover level). Vegetated non-treed classes comprised bryoids, herbs, wetland, and shrubs. Vegetated treed land cover classes included wetland-treed, coniferous, broadleaf, and mixed wood. Independent validation of the land cover maps indicated an overall accuracy of 70.3% ± 2.5%.

Wall-to-wall, 30-m forest structure metrics (i.e., Lorey's height, total aboveground biomass, elevation covariance, and canopy cover) were also annually derived from the BAP composites using the imputation method described in Matasci et al. [@matasciThreeDecadesForest2018; -@matasciLargeareaMappingCanadian2018]. This method uses lidar and field plot data to estimate forest structure metrics from topographic and Landsat spectral predictors, using a k-Nearest Neighbor approach. Reported accuracy for the structure metrics indicated a RMSE% ranging from 24.5% to 65.8% and a R^2^ ranging from 0.125 to 0.699 [@matasciThreeDecadesForest2018].

Forest cover classes (deciduous, broadleaf, mixed-wood, and wetland-treed) were used to generate land cover masks to restrict the comparison of forest structural attributes to treed pixels. Pixels with harvest activity disturbances detected post-1985 were also removed from forest structural attribute rasters in both PA and UA, in order to restrict analysis to non-anthropogenically disturbed areas. All datasets are displayed in @fig:data-fig.

![Figure 2: Visualizations for all layers included in the analysis for Garibaldi Park and surrounding region (red outline) in BC for 2015.](figures/data_map.png){#fig:data-fig}

## Analysis

To determine bias in ecosystem representation in BC's PA network, we compared BEC zone, land cover, and disturbance proportions within and outside the PA network. We employ counterfactual thinking by examining BEC zone, and land cover as a function of elevation, and secondly compiled disturbance rates on a latitudinal gradient across the province. Forest structural attributes were then examined at a finer ecosystem classification level, statistically comparing PA vs UA across similar ecosystems. Forest structural means across BC zones were calculated to determine which forest structures need additional representation in the current BC PA network. All data manipulation and analysis was conducted in the **R** [@R-base] or **Python** programming languages.

### Ecosystems, Land Cover, and Disturbances

BEC zones and land cover classifications were aggregated to both PA and UA in order to determine the proportion of each zone under the protected classifications, to examine progress towards the Aichi biodiversity targets. In this analysis, zones were used to examine categorical data (land cover and disturbance) for the period of 1984-2019. Land cover and BEC zones were further examined along an elevation gradient, at 50m increments. Histograms of area by elevation were generated in order to examine the areal magnitude alongside the proportional coverage of land cover and BEC zones. This allows us to examine the amount of area protected at each elevation, as well as the differences between PA and UA. Forest disturbances (including harvesting) were aggregated along a latitudinal gradient at increments of 0.5°.

### Forest Structural Attributes

T-tests for PA vs UA were conducted on all pixels selected for analysis by BEC subzone and forest structural attribute for 2015, and the Bonferroni correction was applied. The Bonferroni correction avoids spuriously significant results in multiple comparison tests by dividing the significant p-value (0.01) by the number of tests [@bonferroni1936]. Within each BEC zone, higher proportions of significant tests will indicate dissimilar subzones in each forest structural attribute. The mean values for PA and UA forest structural attributes were calculated, in order to examine the differences in their distribution and determine which structures and zones differ between PA and UA. Values were also converted into z-scores to determine the greatest standardized vector magnitude when comparing canopy cover, elevation covariance, and forest height between PA and UA.

# Results

### Ecosystems, Land Cover, and Disturbances



British Columbia's ecosystems are protected at varying rates across the province (@fig:bec-conch). Of the 16 ecosystems present in BC, seven are protected at rates above the Aichi biodiversity target (17%). Only two zones (Boreal Altai Fescue Alpine and Interior Mountain-heather Alpine) are currently protected at rates above the Canadian 2025 protection targets (25%). Zones with Douglas-fir (*Pseudotsuga menziesii*) as dominant old-growth components (Coastal Douglas-fir and Interior Douglas-fir) are the least proportionally represented zones in British Columbia, with 4.9% and 6.4% protected, respectively (@fig:bec-conch).

![Figure 3: Areal proportion of biogeoclimatic ecosystem classification (BEC) zones protected in British Columbia (See Table 1 for full BEC zone names).](figures/bec_bar.png){#fig:bec-conch}

As elevation increases in BC, increasing terrestrial area is protected within the PA network until \~4000m, upon which all terrestrial area is protected (@fig:bec-elev). When comparing between PA and UA, zones are protected at differing proportions. Zones commonly found at high elevations, such as the Boreal Altai Fescue Alpine, are predominantly located in protected areas, however, little terrestrial area is found at these elevations. In low elevations, proportions of area protected also differ, with Coastal Western Hemlock having a large proportion of coverage in PA, while in UA, Boreal Black and White Spruce are underrepresented. Generally, the remaining ecosystems are found at similar rates in both PA and UA (@fig:bec-elev).

![Figure 4: Histogram of area protected in British Columbia by Elevation (a). Proportion of Biogeoclimatic Ecosystem Classification (BEC) zone by elevation for both protected areas (b), and unprotected areas (c). Histogram of area unprotected in British Columbia by Elevation (d).](figures/bec_elev_hist.png){#fig:bec-elev}

Protected land cover also varies by proportion (@fig:vlce-conch). Non-vegetated classes of snow/ice, exposed/barren land, and rock/rubble have higher than average proportions protected while mixed wood and broadleaf land cover classes are underrepresented. All other classes are found at rates similar to the overall proportion of the province protected (\~15%; @fig:vlce-conch).

![Figure 5: Areal proportion of land cover classes protected in BC.](figures/vlce_bar.png){#fig:vlce-conch}

Similar to BEC zones (@fig:bec-elev), land cover also varies with elevation (@fig:lcc-elev). Expectedly, snow/ice make up a large proportion of PA at higher elevations. At lower elevations in UA, mixed wood forest is a more common forest type than in PA, while wetland classes (wetland, wetland-treed) are less frequent in the 400-900m elevation range in UA compared to PA.

![Figure 6: Histogram of area protected in British Columbia by Elevation (a) Proportion of land cover by elevation for both protected areas (b), and unprotected areas (c). Histogram of area unprotected in British Columbia by Elevation (d).](figures/lcc_elev_hist.png){#fig:lcc-elev}

Examining the elevation distributions of BEC zones and land cover classes shows elevation variation in some classes and ecosystems (@fig:elev-boxplots). Generally, BEC zones are found at similar elevation profiles in both PA and UA. Alpine BEC zones (Interior Mountain-heather Alpine, Boreal Altai Fescue Alpine, and Coastal Mountain-heather Alpine) are found at similar elevations across PA and UA, while other zones such as Sub-Boreal Pine -- Spruce, Ponderosa Pine, and Bunchgrass vary in their elevation profiles. Land cover classes show differences in the wetland, wetland-treed, and mixed wood classes. The wetland classes are found at lower elevations in PA than UA, while the mixed wood class has more variation in PA.

![Figure 7: Elevation boxplots for BEC zones (a), and land cover classes (b). Whiskers indicate first quartile minus the interquartile range and third quartile to the interquartile range. Box and interior vertical line indicate first quartile, median, and third quartile, respectively.](figures/elev_boxplots.png){#fig:elev-boxplots}

Overall, the burned area of forested cells is similar between PA (2.5% overall) and UA (2.3%), while harvesting is much higher in UA (7.2%) than in PA (0.33%). Harvesting is more common at lower latitudes in UA than at higher latitudes. Fire shows similar, but not identical patterns across varying latitudes, with higher wildfire proportions at high latitudes and between 51-53°N (@fig:lat-dist).

![Figure 8: Proportion of area disturbed by latitude from 1984 to 2019 in protected areas (a), and unprotected areas (b). Proportion of terrestrial area that is protected at each latitude (c).](figures/latitude_disturbance_plot.png){#fig:lat-dist}

### Forest Structural Attributes

@fig:t-test-plot shows the subzonal proportional significance (*p \< 0.01*) grouped by ecosystem for the 496 comparisons of forest structural variables. Higher percentages confirm ecosystems which had increased number of dissimilar subzones for the specific indicator, and shows that at least half of all subzones in each ecosystem are significantly different (the exception being Ponderosa Pine, which consists of a single subzone that is not significantly different in canopy structure). Median proportional significance values for canopy height, canopy cover, and aboveground biomass are universally significantly different between PA and UA within the same ecosystem.

![Figure 9: Boxplot of proportion of ecosystem subzone which have significant p-values from a two-tailed t-test with the Bonferroni correction (n = 496) applied at a significance level of 0.05. Boxplot vertical lines indicate the first quartile, the median, and the third quartile. The whisker extends from the first quartile to the smallest value no further than 1.5 * interquartile range from the first quartile.](figures/t_tests_scatter.png){#fig:t-test-plot}

Forest structural attributes vary between PA and UA in BC (@fig:structure-3d-scatter). The largest differences between PA and UA are found in canopy structure in the Coastal Douglas-fir BEC zone, with the protected area having much higher canopy structure values. As shown in @fig:t-test-plot, forests are commonly significantly different when comparing PA vs UA across all attributes. When examining the forests on an BEC zone level, only one BEC zone has a \>5% difference in vertical forest structure (co-efficient of variation in vegetation returns), six BEC zones have \>5% difference in canopy cover, and five BEC zones have a \>5% difference in canopy height. Ponderosa pine has large differences in canopy cover and canopy height (\>5%), but minor differences in elevation covariance (only 0.25%; Table 2). PA in the Ponderosa Pine, Interior Mountain Heather Alpine, and Coastal Douglas-fir have more aboveground biomass than in UA in corresponding areas (@fig:structure-3d-scatter).

![Figure 10: Z-Scores of forest structural attributes in PA, UA, and their differences across BEC zones in BC.](figures/fstruct_zscores.png){#fig:structure-3d-scatter}

# Discussion

The recent global availability of freely available, open-source, consistent, and accurate remote sensing data products allow researchers to examine issues of representation of PA compared to UA, and regional ecosystems in novel ways [@boltonUncoveringRegionalVariability2019; @soverelCharacterizingForestFragmentation2010; @hansenTrendsVitalSigns2018]. Additionally, the capacity to track forest structural attributes, a key indicator of forest biodiversity [@guo2017], across wide swaths allows for informed decisions on potential locations of new PA which capture previously underrepresented forest structure conditions [@noss1999]. By applying this analysis to an entire PA network across BEC zones (or other ecological classifications), it becomes possible to determine not only which BEC zones need additional representation (the proportional metric), but also what types of forest structures should be represented to ensure adequate biodiversity protection [@lemieux2005].

Internationally, biodiversity preservation targets aim to protect a proportion of the total terrestrial area [@cbd2010]. Frequently, new protected areas are placed in high-elevation, low-productivity ecosystems both globally [@venter2014; @joppa2009; @venter2018], and in BC, as confirmed by our analysis of ecosystem (@fig:bec-conch) and land cover (@fig:vlce-conch) proportions. Alpine ecosystems are more commonly protected (@fig:bec-conch), as are the land covers commonly present within them (rock/rubble, snow/ice, exposed/barren land; @fig:vlce-conch). As elevation increases, these ecosystems and land covers begin to dominate the proportional representation (see @fig:bec-elev and @fig:lcc-elev). Differences between elevation profiles in land cover classes and BEC zones were also found, with the starkest difference being that wetland classes were found at lower elevations in PA (@fig:elev-boxplots)

In high elevation ecosystems, Boreal Altai Fescue Alpine dominates the PA proportions above 3000m, replacing the Coastal Mountain-Heather Alpine ecosystem found in UA (@fig:bec-elev). These zones were both protected at rates above the average (@fig:bec-conch), and above the Aichi biodiversity targets. Interior mountain-heather alpine had large differences in canopy cover and canopy height, while Boreal Altai Fescue Alpine only showed large differences in height. The Coastal Mountain-heather Alpine did not any have large forest structural attribute differences (Table 2).

Distribution of disturbances followed a similar pattern to that reported by @boltonUncoveringRegionalVariability2019. Thus, the area affected by wildfires is comparable between PA and UA and at mid latitudes (51-53°N), while harvesting activity is more prevalent in UA and at low latitudes (@fig:lat-dist).

Our analysis shows that the majority of structural attributes were significantly different between the protected and unprotected forest stands across BEC subzones (@fig:t-test-plot). In the south, Coastal Douglas-fir, a zone with a single subzone, had the large variation between PA and UA in two of four forest structural attributes examined. The unprotected forests were significantly less tall, had significantly less canopy cover, and significantly higher elevation covariance (vertical forest structure; @fig:structure-3d-scatter). In addition, it was the least protected BEC zone by area, with only 4.9% of the total terrestrial area protected. In this specific BEC zone, not only does additional area need to be protected to meet national goals, different forest structures need to be included in new protected areas [@paillet2010].

Utilizing this information on the proportion of BEC zones protected (@fig:bec-conch), as well as their forest structural attributes (Table 2), it is possible to identify which forest structures need to be added to the PA network in BC. Those BEC zones with large differences (identified as being \>5% change from PA to UA) suggest additional protection is needed to encapsulate these underrepresented forest structures. For example: the forests in the Bunchgrass zone have large differences in both canopy cover and canopy height, with the PA having larger values in both attributes (Table 2). New PA in this BEC zone should contain forests with shorter and more open forests. A future avenue of research could be to incorporate forest structural attributes into spatially optimized PA placement approaches [@christensen2009].

The advent of free and open-source global datasets can allow for the monitoring of protected area health across the globe [@nagendraRemoteSensingConservation2013]. Analyzing large amounts of free and open-source data using open-source software approaches offers previously unseen perspectives into protected area representativeness. There are some challenges associated with this, namely: optical imagery archives being scarce in some regions due to imagery acquisition policies [@wulder2016], clouds and atmospheric interference, lack of aerial lidar data available, and varying hierarchies of land cover classifications in differing regions. New data and satellite missions are being introduced that can meet these challenges at a spatial resolution of 30 m or less such as Landsat-9 and Sentinel-2, as well as spaceborne lidar such as GEDI [@dubayahGlobalEcosystemDynamics2020] and ICESat-2 [@neuenschwander2020], which can provide global coverage of various forest structural attributes [@potapovMappingGlobalForest2021] through similar imputation methods to @matasciThreeDecadesForest2018, global land cover maps [@potapovLandsatAnalysisReady2020; @zanagadaniele2021], and forest disturbance maps [@hansenHighResolutionGlobalMaps2013]. These novel datasets provide clear opportunities for regional to global analyses of PA vs UA to be conducted concerning forest structure.

Future research monitoring protected area health using satellite remote sensing could focus on implementing essential biodiversity variables [@pereira2013] into their monitoring scheme. Advancing research towards these variables would not only benefit PA monitoring projects, but also biodiversity monitoring projects across the globe. Beyond this, examining the recovery of forest structural attribute following disturbances in both PA and UA could assess the effectiveness of PA for promoting regeneration.

# Conclusion

In conclusion, we identified biases in the BC PA network for PA to be placed in high-elevation BEC zones, commonly dominated by low-productivity land covers. We examined the disturbance regimes of PA vs UA by latitude, finding that wildfires are similar, while harvesting differs across the province. We then compared the forest structural attributes across all BEC subzones, finding that the majority of subzones have significantly different forest structures. Beyond this, we identified BEC zones with large variation in mean forest structural attributes. When new PA locations are decided upon in BC, they should take forest structure into consideration, as wall-to-wall coverage of forest structural attributes becomes available. Novel datasets can allow this methodology to be applied across large regions, in order to identify PA biases and underrepresented forest structures.

\newpage

# Acknowledgments

This research was funded through the Living Lab for Climate Change and Conservation program of the British Columbia Parks (grant ID: TP21JHQ011) and in part by NSERC support of Coops (RGPIN-2018-03851). Remote sensing data products utilized in this research are free and open and available for download at: <https://ca.nfis.org/maps_eng.html>. We thank Dr Michael Wulder and Dr Joanne White for development and early access to these National Terrestrial Ecosystem Mapping System (NTEMS) products. We also thank an anonymous reviewer for their comments which helped improve the manuscript.

# Literature Cited
