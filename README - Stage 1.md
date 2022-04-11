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
* Proses selanjutnya perlu dilakukan transformasi agar data nya berdistribusi normal.  Penghapusan data outlier.

C. Multivarate Analysis 
* Berdasarkan heatmap chart, terdapat beberapa feature yang memiliki korelasi dengan label yaitu feature previously_insured, vehicle damage dan policy_sales_channel dimana keterkaitan antara feature dengan label dijabarkan dalam pemaparan berikut:
  * Ada kaitan yang cukup kuat antara feature previously_insured dengan label. Dimana semakin besar nilai previously_insured maka semakin kecil pula nilai label nya. Sehingga feature ini tetap perlu dipertahankan. 
  * Feature vehicle damage memiliki kaitan yang lumayan kuat dengan label. Dimana feature ini memiliki nilai korelasi sebesar 0.4 (mendekati 0.7). Feature ini dapat dipertahankan untuk pembuatan model.
  * Feature policy_sales_channel memiliki korelasi dengan label. Walaupun nilai korelasi anntara feature dengan label ini tidak sebesar feature lainnya. Namun feature ini dapat tetap dipertahankan karena in real life, sales channel dapat mempengaruhi keputusan nasabah untuk tergabung dengan program baru yang ditawarkan.
* Berdasarkan plot pada uji multivariat, untuk distribusi response mayoritas customer merespon tidak tertarik (0). pada variabel umur kendaraan (Vehicle_Age) mayoritas < 1 tahun dan 1-2 tahun. kemudian mayoritas customer memiliki surat izin mengemudi (Driving_License). untuk variabel Vehicle_Age dan Driving_License, perlu diperhatikan dalam langkah selanjutnya karena datanya imbalance.
