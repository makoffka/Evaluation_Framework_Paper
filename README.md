# Evaluation_Framework_Paper

I have used 3 datasets: Cirrhosis, Diabetes and Stroke. They are in the Data folder
I had 4 models: TVAE, CTGAN, GReaT, and RTF
2 of them TVAE and CTGAN - are very quick and easy to run from VScode. 
RTF and GReaT require more resources and I was running them on Google Colab with T4.
I repeated the same evaluation process for each of them.
In addition I did TSTR where I took generated Synthetic data and used as a Training data to see if the Fake data is useable for the downstream tasks.
Then I did the same evaluation only for TSTR dataset - trained on synthetic tested on real testing data.

I also checked each synthetic dataset for out of range values using great_expectations package. 
I think I did it separately - due to that it's not included in the code provided except for RTF_cirrhosis (It throws an error there. Likely due to some change in the package. It worked in May)
