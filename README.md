# Tugas3-Machine-Learning-2108107010017

Dataset SVC : Prediksi obesitas
Link dataset : https://www.kaggle.com/datasets/danielkyrka/bmw-pricing-challenge

Adapun Atributnya adalah:

Age: The age of the individual, expressed in years. Gender: The gender of the individual, categorized as male or female. 
Height: The height of the individual, typically measured in centimeters or inches. 
Weight: The weight of the individual, typically measured in kilograms or pounds. 
BMI: A calculated metric derived from the individual's weight and height 
PhysicalActivityLevel: This variable quantifies the individual's level of physical activity 
ObesityCategory: Categorization of individuals based on their BMI into different obesity categories SVR

Dataset ini berisi kondisi tubuh seseorang dengan berbagai level obesitas. Tujuan dari dataset ini dapat memprediksi tingkat obesitas pada manusia

Dataset SVR : BMW Pricing Challenge
Link Dataset : https://www.kaggle.com/datasets/danielkyrka/bmw-pricing-challenge

Adapun Atributnya adalah:
maker_key
model_key
mileage
engine_power
registration_date
fuel
paint_color
car_type
feature_1
feature_2
feature_3
Dataset merupakan penjualan mobil bermerek BMW dengan spesifikasi mobil beserta harganya. Tujuan dari dataset ini dapat memprediksi harga jual mobil MBW berdasarkan spesifikasinya

## Klasifikasi
1. Menyiapkan library yang diperlukan
2. Melakukan preprocessing
3. Menerapkan metode SVC pada dataset
4. Menerapkan metode klasifikasi menggunakan ANN
5. Melihat akurasi

Dilakukan perbandingan model SVC dengan model ANN. Adapun perbandingannya adalah:
- Model SVC:
Akurasi menggunakan tinggi dan berat badan untuk memprediksi tingkat obesitas adalah 98.4%
Akurasi menggunakan BMI dan berat badan untuk memprediksi tingkat obesitas adalah 97.6%
Akurasi menggunakan PhysicalActivityLevel dan berat badan untuk memprediksi tingkat obesitas adalah 68.6%

-Model ANN:
Akurasi menggunakan tinggi badan, berat badan, BMI, dan PhysicalActivityLevel untuk memprediksi tingkat obesitas adalah 98.13% dengan menggunakan epoch 100

Epoch 98/100
24/24 [==============================] - 0s 2ms/step - loss: 0.1886 - accuracy: 0.9787
Epoch 99/100
24/24 [==============================] - 0s 2ms/step - loss: 0.1864 - accuracy: 0.9747
Epoch 100/100
24/24 [==============================] - 0s 2ms/step - loss: 0.1836 - accuracy: 0.9813

Dari perbandingan 2 model tersebut dapat dilihat SVM dan ANN menghasilkan akurasi yang hampir sama, akan tetapi pada model SVC penggunaan sebuah fitur dapat mempengaruhi nilai akurasi

## Regresi
1. Menyiapkan library yang diperlukan
2. Melakukan preprocessing
3. Menerapkan model SVR pada dataset
4. Menerapkan metode Regresi menggunakan ANN
5. Melihat akurasi RMSE
6. Menampilkan visualisasi

Dilakukan perbandingan RMSE pada model SVR dengan model ANN. Adapun perbandingannya adalah:
- Model SVR: 
RMSE model polynomial dengan degree 3 menggunakan fitur engine_power untuk memprediksi harga mobil sebesar: 0.7154030320522825
RMSE model polynomial dengan degree 3 menggunakan fitur mileage untuk memprediksi harga mobil sebesar: 0.8439685619772759

- Model ANN: 
RMSE model ANN menggunakan fitur engine_power untuk memprediksi harga mobil sebesar: 7649.869641718357
RMSE model ANN menggunakan fitur mileage untuk memprediksi harga mobil sebesar: 7680.162968872658
