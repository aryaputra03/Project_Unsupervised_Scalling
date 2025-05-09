
![1_W2B0ZbRU_wuLrldN5Ak_5A](https://github.com/user-attachments/assets/8e380fed-4b1a-4714-ae55-7f65ef851304)

Dalam pengembangan model machine learning, salah satu langkah penting dalam preprocessing adalah feature scaling. Teknik ini bertujuan untuk menyeragamkan skala antar fitur guna meningkatkan performa model, terutama pada algoritma yang sensitif terhadap skala seperti K-Nearest Neighbor (KNN) dan Support Vector Machine (SVM). Teknik umum yang digunakan meliputi MinMaxScaler, StandardScaler, dan RobustScaler, dengan keunggulan masing-masing, terutama dalam mengatasi outlier.

Eksperimen ini membandingkan empat metode scaling (MinMax, Standard, Robust, dan tanpa scaling) pada lima algoritma: Linear Regression, SVM, KNN, Random Forest, dan CatBoost. Evaluasi dilakukan dengan cross-validation sebanyak 25 kali, menghasilkan 100 titik evaluasi per kombinasi. Performa diukur menggunakan Mean Squared Error (MSE), dan dianalisis secara statistik dengan Mann-Whitney U Test untuk menilai signifikansi perbedaan antar metode.

Hasil menunjukkan pengaruh penskalaan bervariasi antar model. Pada Linear Regression, dampaknya minimal namun penskalaan tetap disarankan. KNN sangat bergantung pada skala, sehingga penskalaan krusial untuk akurasi. SVM menunjukkan peningkatan performa dalam skenario tertentu, khususnya dengan StandardScaler. Random Forest dan CatBoost relatif tidak terpengaruh oleh penskalaan, tetapi tetap bisa diterapkan demi kestabilan pipeline.
