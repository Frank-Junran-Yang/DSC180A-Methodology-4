# DSC 180A Methodology Assignment 4

**Name:** Junran Yang
**Email:** juy029@ucsd.edu
**Section:** D16
**Mentor:** Dr. Rob Knight

**1. What is the most interesting topic covered in your domain this quarter?**

The most interesting topic for me is how we can use DNA from ocean microbes to measure the health of the ocean. In the paper I replicated (Martiny et al., 2026), the authors use metagenomes of Prochlorococcus to build a genomic stress index that shows which nutrients are limiting, and then combine it with satellite data to map nutrient stress across the whole ocean. Coming from a math and data science background with no biology, it was surprising to see that genes in tiny bacteria can tell us about ocean conditions at a global scale.

**2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

In Quarter 1, I replicated the paper's analysis starting from the authors' already-computed stress index values. For Quarter 2, I would like to recompute the genomic stress index directly from the raw metagenome reads for a subset of samples (around 12 samples), following the method from Ustick et al. (2021), and check whether my values match the authors' values. If that works, I would test whether the relationship between the genomic stress index and the satellite data still holds when the stress index is rebuilt independently.

**3. What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

Right now, my replication starts from the authors' processed data, so it only checks whether their analysis gives the same numbers, not whether the data was built correctly. I would change this by going back to more of the raw data, for example using the World Ocean Atlas nutrient data directly (the server was down when I tried, so Fig. 1A was not replicated). I would also look more closely at the parts that did not match, like the iron result in Fig. 1C, where my result had the opposite sign from the paper.

**4. What other techniques would you be interested in using in your project?**

I would like to try other machine learning models besides random forest, such as gradient boosting, and use SHAP values to explain which features matter most for predicting nutrient stress. I am also interested in learning bioinformatics tools for mapping metagenome reads to reference genomes, since that is needed to recompute the stress index. Finally, I would like to use spatial cross-validation, because ocean samples that are close to each other are not independent.
