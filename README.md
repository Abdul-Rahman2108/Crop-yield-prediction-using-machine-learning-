**_Crop Yield Prediction based on Indian Agriculture using Machine Learning_**

**ABSTRACT**
_In India, we all know that Agriculture is the
backbone of the country. This paper predicts the yield of almost
all kinds of crops that are planted in India. This script makes
novel by the usage of simple parameters like State, district,
season, area and the user can predict the yield of the crop in
which year he or she wants to. The paper uses advanced
regression techniques like Kernel Ridge, Lasso and ENet
algorithms to predict the yield and uses the concept of Stacking
Regression for enhancing the algorithms to give a better
prediction._

EXISTING SYSTEM

Ananthara, M. G. et al. (2013, February) proposed a
prediction model for datasets pertaining to agriculture which is
called as CRY algorithm for crop yield using beehive
clustering techniques. They considered parameters namely crop
type, soil type, soil pH value, humidity and crop sensitivity.
Their analysis was mainly in paddy, rice and sugarcane yields
in India. Their proposed algorithm was then compared with C&R tree algorithm and it outperformed well with an accuracy
of 90 percent 
[2]. Awan, A. M. et al. (2006, April) built a new,
smart framework focused on farm yield prediction clustering
kernel methodology and they considered parameters like
plantation, latitude, temperature and precipitation of rainfall in
that latitude. They had experimented weighted k-means kernel
method with spatial constraints for the analysis of oil palm
fields 
[3]. Chawla, I. et al. (2019, August) used fuzzy logic for
crop yield prediction through statistical time series models.
They considered parameters like rainfall and temperature for
prediction. Their prediction was classification with levels
‘good yield’ , ‘very good yield’ 
[4]. Chaudhari, A. N. et al.(2018, August) used three algorithms namely clustering kmeans,
Apriori and Bayes algorithm, then they hybridized the
algorithm for better efficiency of yield prediction and they
considered parameters like Area, Rainfall, Soil type and also
their system was able to tell which crop is suitable for
cultivation based on the mentioned features 
[5]. Gandge, Y.(2017, December) used many machine learning algorithms for
different crops. They studied and analyzed which algorithm
would be suitable for which crop. They have used K-means,
Support vector Regression, Neural Networks, C4.5 Decision
tree, Bee-Hive Clustering, etc. The factors implying were soil
nutrients like N, K, P and soil ph. 
[6]. Armstrong, L. J. et al.(2016, July) used ANNs for the prediction of rice yield in the
districts of Maharashtra, India. They considered climatic
factors namely (considering range) temperature, precipitation
and reference crop evapotranspiration. The records were
collected from Indian Government repository from 1998 to
2002 
[7]. Tripathy, A. K. et al. (2016, July) were same authors
who used support vector machines to predict the rice crop yield
with same features as the previous paper mentioned 
[8]. Petkar,O. (2016, July) were also the same authors who applied for
SVM and neural networks for rice crop yield prediction
proposed a new decision system which is an interface to give
the input and get the output 
[9]. Chakrabarty, A. et al. (2018, December) analyzed crop prediction in the country of
Bangladesh where they majorly cultivate three kinds of rice,
Jute, Wheat, and Potato. Their research used a deep neural
network where the data had around 46 parameters into their
consideration. Few of them were soil composition, type of
fertilizer, type of soil and its structure, soil consistency,
reaction and texture.

**_PROPOSED SYSTEM_**
**Pre-processing**
For the given data set, there are quite a few ‘NA’ values   which are filtered in python. Furthermore, as the data set consists of numeric data, the proposed system used robust scaling, which is quite similar to normalization, but it instead uses the inter quartile range whereas normalization is something which normalization shrinks the data in terms of 0 to 1.

**Stacked Regression:**

This is a kind of ensembling but a little of enhancement of averaging. In this, we add a meta model and use the out of fold predictions of the other models used to train the main meta model.
Step-1: the total training set is again divided into two different sets. (train and holdout)
Step-2: train the selected base models with first part (train).
Step-3: Test them with the second part. (holdout)
Step-4: Now, the predictions obtained from test part are inputs to the train higher level learner called meta-model.

**Advantages**
In the proposed system,an effective  advanced regression techniques used – Lasso, ENet and Kernel Ridge and further.
To The system is more effective due to presence of Data Sets Classification Techniques.

