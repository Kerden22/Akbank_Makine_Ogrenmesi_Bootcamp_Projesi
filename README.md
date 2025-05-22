
# Credit Card Fraud Detection - ML Bootcamp Project 

## 🚀 Proje Amacı

Bu proje, kredi kartı ile yapılan işlemler arasından dolandırıcılık içerenleri tespit etmeye yönelik bir makine öğrenmesi çalışmasıdır. Proje, Akbank ML Bootcamp kapsamında gerçekleştirilmiştir ve gözetimli öğrenme tekniklerini kullanarak sınıflandırma modeli geliştirmeyi hedeflemiştir.

## 📁 Kullanılan Veri Seti

-   **Kaynak:** [Kaggle - Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
    
-   **Boyut:** 284,807 işlem kaydı
    
-   **Sınıflar:** 0 (Normal), 1 (Dolandırıcılık)
    
-   **Özellikler:** Zaman, Tutar ve PCA ile dönüştürülmüş V1-V28 aralığında anonimleştirilmiş nitelikler
    

## 📊 Veri İncelemesi (EDA)

-   Sınıf Dağılımı: Veri %99.8 oranında normal işlemlerden oluşmaktadır.
    
-   Korelasyon Matrisi: Özellikler arasındaki ilişkiler incelendi.
    
-   Zaman vs. Sınıf: Dolandırıcılık işlemleri belli zaman aralıklarında yığılmakta.
    

## ⚖️ Veri Ön İşleme

-   **Eksik Veri:** Yok
    
-   **Sınıf Dengesizliği:** SMOTE ile over-sampling uygulandı
    
-   **Özellik Ölçekleme:** `StandardScaler` ile tüm modeller için
    
-   **Train/Test Ayrımı:** %80 / %20 oranında stratified
    

## 🧐 Uygulanan Modeller ve Sonuçlar

Sıra

Model

Accuracy

1

Random Forest

0.9994

2

XGBoost

0.9994

3

CatBoost

0.9987

4

K-Nearest Neighbors

0.9980

5

Logistic Regression

0.9899

6

Naive Bayes

0.9751

> ✅ En başarılı modeller Random Forest ve XGBoost olmuştur.

## 🎓 Hiperparametre Optimizasyonu

-   **Yöntem:** GridSearchCV
    
-   **Uygulanan Modeller:** Random Forest, XGBoost
    
-   **Amaç:** F1 skorunu maksimize edecek parametre kombinasyonunu bulmak
    

## 🎯 Değerlendirme Metrikleri

-   Confusion Matrix, Accuracy, Precision, Recall, F1-score değerleri detaylı olarak raporlandı.
    
-   Dîngesiz sınıf yapısı nedeniyle F1 skoruna öncelik verildi.
    


## ✨ Gerçek Hayat Uygulaması

Bu proje, bankacılık ve e-ticaret gibi alanlarda kredi kartı işlemlerinin otomatik takibi için kullanılabilir. Gerçek zamanlı sahtekarlık tespiti sistemlerinin temelini oluşturabilir.

## ✏️ Geliştirme Önerileri

-   ✔ ROC-AUC grafik analizleri ile model karar eğikleri incelenebilir.
    
-   ✔ Daha gelişmiş topluluk modelleri (ensemble) denenebilir.
    
-   ✔ Model deploy edilerek bir web arayüzde sunulabilir.
    
-   ✔ Aynı veri seti ile K-Means gibi gözetimsiz yöntemler uygulanabilir.
    

----------

📅 Proje, Akbank ML Bootcamp 2025 kapsamında gerçekleştirilmiştir.

## Mahmut Kerem Erden - k.erden03@gmail.com
