<!-- PROJECT LOGO -->
<br />
<p align="center">

  <h3 align="center">Predict Future Sales</h3>

  <p align="center">
    DSAI Final
    <br />
    <a href="https://drive.google.com/file/d/1S-Z8nW06R4dPNLm3soxhVm5dB_KgDFM3/view?usp=sharing"><strong>Slidecs »</strong></a>
    <br />
  </p>
</p>


## data preprocessing

1. Check missing values
2. Remove outliers
3. Check anomalies 
    * 我認為退貨行為屬正常現象，因此決定保留商品銷量負值
4. Combine duplicated feature values
5. Feature construction


## feature construction

* From  **shop_name**  generate  **latitude**, **longitude**, and **area code**.
* From  **item_category_name**  generate  **category** and **subcategory**.
* Add month related features.
* Add lag features


## model comparison

Models | validation MSE | test MSE
--- | --- | --- | 
XGBoost | 0.836 | **0.888** |
GBDT | 1.000 | 1.038 |
LightGBM | 1.004 | 1.039 |


## rank on [kaggle](https://www.kaggle.com/competitions/competitive-data-science-predict-future-sales)

* Public Leader Board: 1918/14909 (Top 13%)
* Public Score: 0.88801


## conclusion

* The most important thing is **exploratory data analysis**.
* Understanding the **information**, **structure** and **characteristics of data** can makes our model better. 



<!-- CONTACT -->
## Contact

About me: [Hsin-Hsin, Chen](https://www.facebook.com/profile.php?id=100004017297228) - shulammite302332@gmail.com
