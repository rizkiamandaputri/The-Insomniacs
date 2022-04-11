# The-Imsoniacs
Health Insurance Sell Cross Prediction

Stage 1 <br>
A. Descriptive Statistics
* Semua tipe data pada kolom sudah sesuai dan tidak terdapat missing values sehingga tidak berlu diubah
* Terdapat beberapa kolom yang diduga ada keanehan timpang sehingga perlu diolah terlebih dahulu atau tidak digunakan  
* Target output dari project ini adalah memprediksi respons user apakah tertarik atau tidak untuk mendaftar asuransi kendaraan

B. Univariate Analysis
* Terdapat outlier pada varibel Annual_Premium.  
* Secara visualisasi tidak ada data yang berdistribusi normal.  Variabel Age memiliki positively skewed  
* Variabel vintage berdistribusi uniform  
* Variabel annual_premium berdistribusi bimodal  
* Berdasarkan countplot categorical, untuk distribusi response mayoritas customer merespon tidak tertarik (0). pada variabel umur kendaraan (Vehicle_Age) mayoritas < 1 tahun dan 1-2 tahun. kemudian mayoritas customer memiliki surat ijin mengemudi (Driving_License). untuk variabel Vehicle_Age dan Driving_License, perlu diperhatikan dalam langkah selanjutnya karena datanya imbalance.

