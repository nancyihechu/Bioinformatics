# Bio-informatics
### Data selections and storage
Bio activity data for SARS coronavirus 3C-like proteinase.<br>
In this project, only bio-activity data for coronavirus 3C proteinase (CHEMBL3927) that have IC50 values in nM nanomolar unit was selected to be analysed. 
The Bio-activity class was futher grouped into "Active", "Inactive", and "Intermediate" based on the standard value concentrations in nanomolar (nM).  <br> Compounds having values of less than 1000 nM were considered to be active while those greater than 10,000 nM were considered to be inactive. As for those values in between 1,000 and 10,000 nM they were referred to as intermediate. this grouping formed a new column named "bioactivity_class" <br>
A new Dataframe was then created comprising of the molecule id number, the canonical smiles, bioactivity class, and standard value columns.
This new modified dataframe was then saved into a CSV file
