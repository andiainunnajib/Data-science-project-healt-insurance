# [Data Science Health Insurance Cross Sell Prediction![image](https://user-images.githubusercontent.com/85381045/141938075-e8159ed8-160c-4995-a92a-be9c7fe38380.png)](https://github.com/andiainunnajib/Data-science-project-healt-insurance) 
* Created a prediction to prredict customer that interested in product ansurance
* Build a model to predict whether policyholders (customers) from last year will also be interested in the Vehicle Insurance provided by the company.
* Find EDA in datasets to get insight valuable data
* Plan a communication strategy to reach those customers and optimize the business model.
* Focused to Purchase Rate

## Table of Contents
* **[Project Background](#project-background)**

* **[Data PreProcessing](#data-preprocessing)**

* **[Exploratory Data Analysis](#exploratory-data-analysis)**

* **[Modeling ML](#modeling-ml)**

* **[Business Insight and Recomendation](#business-insight-and-recomendation)**




### Project Background
  A company that engaged in the insurance sector. Currently, we already have health insurance products and will expand to vehicle insurance.

In this company, we have a Data Science team who asked to build a model to predict whether policyholders (customers) from last year will also be interested in the Vehicle Insurance provided by the company.
The number of vehicle grows linearly with its incident numbers

![image](https://user-images.githubusercontent.com/85381045/142726578-4798b72b-f61c-485c-81e8-78720ea896bb.png)

![image](https://user-images.githubusercontent.com/85381045/142726571-38ed5c76-58fd-4926-bb01-5ad13fb38127.png)

![image](https://user-images.githubusercontent.com/85381045/142726568-b0469d4c-ee2d-48c7-a491-a62fecf98b86.png)

![image](https://user-images.githubusercontent.com/85381045/142726586-34391029-e8f7-4221-9c9f-b39694514983.png)

Source :
https://www.bps.go.id/indicator/17/513/1/jumlah-kecelakaan-korban-mati-luka-berat-luka-ringan-dan-kerugian-materi.html
https://www.bps.go.id/indicator/17/57/1/jumlah-kendaraan-bermotor.html


### Data PreProcessing

![image](https://user-images.githubusercontent.com/85381045/142726770-60c8f8d8-d3e1-47b2-b0a9-bcfe43ca9182.png)

There are not missing values and duplicate data, and columns for gender, id, region code are drop because to decreased ML Bias

for outlier used IQR method and this is before after outlier

![image](https://user-images.githubusercontent.com/85381045/142726948-403335bf-6c9e-490f-8285-36fa13d564fc.png)


Feature encoding using one hot encoding 
![image](https://user-images.githubusercontent.com/85381045/142726980-dcd0881c-6f9e-4d03-96b7-d792d444817d.png)

### Exploratory Data Analysis

![image](https://user-images.githubusercontent.com/85381045/142727032-d7374f6f-946f-45f2-ab4c-a05509f064b4.png)

Vehicle age that more than 2 years is the rarest fact. and most of people are not previously insured
![image](https://user-images.githubusercontent.com/85381045/142727052-a7fb0899-4b3c-4489-8b03-5045cd6f42ad.png)
![image](https://user-images.githubusercontent.com/85381045/142727056-c3ab6c36-e5c3-4f9d-b53d-82dc9efeb2c8.png)

For correlation data
![image](https://user-images.githubusercontent.com/85381045/142727076-2123a564-e355-4c90-b1f6-99ecdcacfc2e.png)

### Modeling ML
Random forest outperformed all other ML models by AUC and F-1 score
![image](https://user-images.githubusercontent.com/85381045/142727094-e67b746e-a421-4725-87d6-920c745b0992.png)

and for feature importance vehicle damage and previously insured are the top strongest factors
![image](https://user-images.githubusercontent.com/85381045/142727126-00184f45-93a9-4da1-9aed-0bf442f24cb0.png)

### Business Insight and Recomendation
Insight :
Highest interest in product among age 41-50 years at 4.17%.

Business Recommendation  :
Main focused in age range 41-50 for product.
![image](https://user-images.githubusercontent.com/85381045/142727140-55011348-9c4d-4f88-a98e-0a9e652df400.png)

 Insight :
Highest positive response customers with a Vehicle Age of 1-2 years at 9.10% and Damage Vehicle at 11.92%

Business Recommendation :
Gain more customers in Vehicle Age 1-2 years 
Gain more customers in Vehicle Damage = Yes


Insight :
High percentage positive response for Annual Premium in range 20,000-40,000. 


Business Recommendation :
Focused product rate for Vehicle Insurance in range 20,000 – 40,000.


![image](https://user-images.githubusercontent.com/85381045/142727167-00d65e82-9e08-4487-82c4-c4f764f7bce2.png)

Insight :
Rendahnya ketertarikan pada produk di kalangan usia muda (20-30)
Ketertarikan pada kalangan 41-50 pada produk lebih baik


Solution Recommendation :
Meningkatkan ketertarikan terhadap asuransi kendaraan bagi kalangan usia muda (20-30 tahun).

Marketing Plan & Strategy :
Memanfaatkan social media sebagai sarana dalam mempromosikan produk dan juga mengedukasi orang-orang akan pentingnya mengasuransikan kendaraannya.


![image](https://user-images.githubusercontent.com/85381045/142727169-6bc9d0ca-285b-46c1-be34-2c163a15ee33.png)
