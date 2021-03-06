# Tanzanian-Water-Pumps-Clustering-and-Classification
For this group project, I performed cluster analysis and classification using Python to predict one of three classes for water pumps; functional, functional but needs repair, and non-functions. I used clustering to find hidden data structures to exploit for fitting individual classification techniques with better results than using the entire dataset. Unfortunately, k-means clustering, DBSCAN, hierarchical clustering, nor OPTICS produced well-defined clusters. The entire dataset was therefore used for fitting classification algorithms. The two classification techniques I was responsible for were k-nearest neighbors and stacked generalization ensemble. For the latter, I combined the best models each group member developed. All the models had a hard time predicting the functional but need repair class. My best model was only able to achieve an accuracy of 76%.

The original dataset came from DrivenData as part of a competition: https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/ 
I uploaded a clean/reduced version used for the analysis. The cleaning process was through the lens of using features that could be used in other countries and be general enough to classify water pumps anywhere in the world. We did not participate in the competition, otherwise, the cleaning process would not have been generalized. 

I have only uploaded my notebooks and not my group members'. However, models from their notebooks are imported as pickles in my stacking classifier notebook. I included the pickle files, but it is possible issues may occur due to their notebooks not being included in the repository. 

There are two clustering notebooks, a slim version and long version. The long version uses all the data and took over 24 hours to run. The slim version is much quicker and only uses 10% of the dataset. The slim version includes the same analysis from the long version plus silhouette plots.

The Python libraries used include matplotlib (3.3.4), NumPy (1.20.1), pandas (1.2.3), pickle, scikit-learn (0.24.1), and warnings
