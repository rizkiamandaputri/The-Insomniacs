# The-Imsoniacs
Health Insurance Sell Cross Prediction

Stage 2
1. Data Cleansing
  * Dari proses tersebut tidak terdapat data null dan data yang duplikat, untuk tipe data semua kolom pun sudah sesuai. 
  * Didapatkan data outlier pada kolom Annual Premium. Kemudian dilakukan penghapusan data outlier berdasarkan IQR dan Z-Score.

2. Feature Transformation
  * Dilakukan standardization dan normalization pada fitur Vintage, karena fitur tersebut tidak terdapat pengaruh dan korelasi terhadap target.
  * Dilakukan log tranformation pada fitur Age dan Annual_Premium karena kedua fitur tersebut memiliki distribusi data yang right-skewd atau memiliki buntut yang panjang di sebelah kanan.

3. Feature Encoding
  * Melakukan label encoding pada data, yaitu : Gender, Vehicle_Age, dan Vehicel_Damage
 
4. Class Imbalance
  * Melakukan undersampling dan oversampling menggunakan teknik SMOTE pada target yaitu Response

5. Feature Engineering
  * Berdasarkan hasil EDA dan dari sisi bisnis, feature yang akan digunakan dalam model adalah : Driving Lisence, Vehicle Damage, Annual Premium, Age, Policy Sales Channel, Region Code, dan Previously Insured. Kemudian untuk feature yang tidak diambil adalah: ID, dan Vintage. Kemudian pada tahap ini dilakukan penambahan feature yang mengktraksi dari data yang ada yaitu :
    * Feature Segment: merupakan klasifikasi customer berdasarkan annual preminya
    * Feature Premi_Rate: merupakan klasifikasi premi berdasarkan umur kendaraannya (Vehicle_Age)
