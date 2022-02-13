# Project description
Prepare a prototype of a machine learning model for Zyfra. The company develops efficiency solutions for heavy industry.
The model should predict the amount of gold recovered from gold ore. You have the data on extraction and purification.
The model will help to optimize the production and eliminate unprofitable parameters.
You need to:
- Prepare the data;
- Perform data analysis;
- Develop and train a model.
  
Data is indexed with the date and time of acquisition (date feature). Parameters that are next to each other in terms of time are often similar.
Some parameters are not available because they were measured and/or calculated much later. 
That's why, some of the features that are present in the training set may be absent from the test set. The test set also doesn't contain targets.
The source dataset contains the training and test sets with all the features.
You have the raw data that was only downloaded from the warehouse. Before building the model, check the correctness of the data.

# Data description
**Technological process**  
`Rougher feed` — raw material   
`Rougher additions` (or reagent additions) — flotation reagents: Xanthate, Sulphate, Depressant  
`Xanthate` — promoter or flotation activator  
`Sulphate` — sodium sulphide for this particular process  
`Depressant` — sodium silicate  
`Rougher process` — flotation  
`Rougher tails` — product residues  
`Float banks` — flotation unit  
`Cleaner process` — purification  
`Rougher Au` — rougher gold concentrate  
`Final Au` — final gold concentrate  

**Parameters of stages**  
`air amount` — volume of air  
`fluid levels`  
`feed size` — feed particle size  
`feed rate`

**Feature naming**  
Here's how you name the features:  
**`[stage].[parameter_type].[parameter_name]`**  
*Example: **rougher.input.feed_ag***  

Possible values for [stage]:  
`rougher` — flotation  
`primary_cleaner` — primary purification  
`secondary_cleaner` — secondary purification  
`final` — final characteristics  

Possible values for [parameter_type]:  
`input` — raw material parameters  
`output` — product parameters  
`state` — parameters characterizing the current state of the stage  
`calculation` — calculation characteristics
