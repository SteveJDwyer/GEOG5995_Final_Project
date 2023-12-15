
 
   GEOG5995_Final_Project_Introduction


     NOTE
   
     The data for this research have been provided by the Consumer Data Research Centre, an ESRC 
     Data Investment, under project ID CDRC ES/L011840/1; ES/L011891/1

    
    PROJECT BACKGROUND
 
    The project question: 
    
 
    Is there a relationship between fuel poverty (FP) and the relative Energy Performance Certificate (EPC)
    scores of English Local Authority Districts (LAD)  
 
    The potential ‘public good’ insight that might be obtained is that if such a relationship is established 
    and it is believed that there is a causal relationship (e.g. lower average EPC LADs contribute to
    higher FP) then the national Government, regional authority or LAD might target resources to improve 
    the EPC ratings of those relatively lower EPC LADs and thereby be more efficient in reducing FP.
    
    DEFINITIONS
  
    FUEL POVERTY (FP) 

    The UK’s Department for Energy Security & Net Zero (DESNZ) determines which households are classified as 
    FP by reference to the Low Income Low Energy Efficiency Rating , that is if the household has: 

    "a property with an energy efficiency rating of band D, E, F or G
    and …its disposable income (income after housing costs (AHC) and energy costs) 
    would be below the poverty line" [FN1]  

    "The poverty line (income poverty) is defined as an equivalised disposable income of less 
    than 60% of the national median" [FN 2]  
  
    KEY DRIVERS FOR FP

    DESNZ[FN 3] sets out the key drivers of FP  as: 
  
    -Energy Efficiency

    - Energy Prices 

    - Incomes 
    
    The project question focuses on the energy efficiency input rather than energy prices and incomes 
    but recognises that whilst energy prices and incomes (via minimum wage or benefit policies) are 
    normally the concern of  central rather than local government there are large regional and
    intra- regional LAD differences  in incomes so FP in LAD is a combination of factors . Separating
    the impact of uneven income distribution within that mix is beyond this paper. 
    
    
    ENERGY PERFORMANCE CERTIFICATES (EPC) AND POTENTIAL EPC (PEPC) SCORES 
    
    EPCs contain scores and ratings for domestic residences in the UK ,the Department for Communities
    and Local Government (DCLG) explains their purpose as follows 
    
    "The EPC will provide an energy efficiency rating from A to G, where A is very efficient 
    and G is the least efficient. The better the rating, the more energy efficient the building is,
    and the lower the fuel bills are likely to be…
    
    Each energy efficiency rating is based on the characteristics of the building itself 
    (the fabric) and its services (such as heating, ventilation and lighting) …
    
    The EPC includes recommendations to help owners and occupiers to improve the energy efficiency 
    of a building. …. The potential rating shown on the EPC is based on all cost-effective 
    recommendations being implemented" [FN 4]
    
   
    Alongside the A- G ratings there is a related score out of 100 so the difference in 
    scores between two residential buildings can be calculated on a very granularly basis i.e. : 
  
    "Energy Performance Certificate (EPC) provides a numerical scale of the theoretical cost of energy
    use in a residential property. This energy performance rating is standardised to a scale of 
    zero (high cost) to 100 (minimal cost), which is frequently used as a measure of energy use of r
    esidential buildings in the UK" [FN 5]
    
    Alongside the EPC score there is a PEPC score that looks at the potential score for the residential 
    property if all the ‘cost-effective’ measures were taken. It does not take into account all possible
    measures  since that might make every potential score 100 ( but at a very high cost).
    
   
    Contents GitHub repository
   
    A 1 :'/Users/user/Documents/GEOG5995-main/rmepc_laua21_mi.csv'
  
    A 2 :'/Users/user/Documents/GEOG5995-main/rmepc_laua21_mo.csv'
      
    B 1 :'/Users/user/Documents/GEOG5995-main/Local_Authority_Districts_December_
          2021_GB_BGC_2022_-350184439094746283.csv'
    
    B 2 :'/Users/user/Documents/GEOG5995-main/LAD_DEC_2021_GB_BGC.shx'
  
    C 1 :'/Users/user/Documents/GEOG5995-main/fuel_poor.csv'
  
    ipynb notebook : GEOG5995M_Final_Project_ID_11489360.ipynb   

    ipynb notebook : GEOG5995M_Final_Project_ID_11489360_Introduction_File.ipynb 
    
    Model evaluation 
   
    R 2  - 0.132 or 13.2% is the percentage of change in the FP(%) or FP(%) variance explainable by the model
    hypotheis.The result is close to 0% (zero explanatory value) than 100% (total expalnatory value). The low 
    value does not suggest a strong fit with the model.
    
    Prob(F-statistic) is very low 4.87e-11(i.e.0.0000000000487) this is much lower than the benchmark value
    of 0.05 which suggest the results are unlikely to be due purely to chance and therefore there is likely 
    to be some relationship between the variables.
    
    Coef(Coeficient) for epc-mi-mo suggests that every one unit change in it will reduce the FP percentage by
    0.7667%,however the confidence intervals ([0.025   0.975]) has a range of 0.545 - 0.988 representing quite 
    a large range. The range around the predicted value (reflecting a weak fit) are positive so not indicative of
    no model relationship.   
   
    Other Findings
  
    The correlation relationship between certain other variables from the data above provide a mixture of 
    useful/confirmatory information and irrelevant ones. In the former category the following points can be 
    made :
  
    1.EPCs and PEPCs appear strongly positively correlated (+0.74). Suggesting that residences with the highest
    EPC scores will also score highly on PEPCs scores, which suggest \"unfairly\" that energy efficient homes 
    are the ones most cost efficient to make even more energy efficient. Although seemingly at first 
    counter-intuitive the  second relationship may partially explain this (as PEPC is is negatively correlated 
    with floor space (-0.15)
    
    2.There is a relative strong inverse realtionship between EPC postion and floor space area (-0.43) which
    is not,suprising as it suggest small homes are more energy efficient than large ones. Although the data 
    does not reveal types of housing one could speculate that English flats are smaller than many English 
    houses and energy efficiency benefits arise from both factors (smaller floor space and less "external" 
    (outside) wall area). Indeed the top EPC ranking of Tower Hamlets and bottom ranking of IoS may be 
    related to the proportion of flats in each LAD.                                           
 
    References
    
    [1] DESNZ (2023) Annual Fuel Poverty Statistics in England,2023(2022 data) 28/2/2023 p6
    
    [2]ibid p6

    [3]ibid p11
    
    [4] Department for Communities and Local Government,'A guide to energy performance certificates for the
    marketing, sale and let of dwellings Improving the energy efficiency of our buildings' (December 2017) 
    Department for Communities and Local Government,  p10
  
    [5] CDRC Residential Mobility and Energy Performance Certificate (RMEPC) Index (LAD Geography) 
    https://data.cdrc.ac.uk/system/files/RMEPC_LA_0.pdf
   
    
