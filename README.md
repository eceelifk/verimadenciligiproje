# Mantar (Mushroom) Sınıflandırması - Veri Madenciliği Dönem Projesi

Bu proje, UCI Machine Learning Repository bünyesinde yer alan **Mushroom** veri seti kullanılarak geliştirilmiş makine öğrenmesi tabanlı bir sınıflandırma ve performans analizi çalışmasıdır.

## Proje Amacı
Mantarların morfolojik ve fiziksel niteliklerine (şapka, koku, solungaç, gövde vb.) dayanarak **yenilebilir (edible - e)** veya **zehirli (poisonous - p)** olarak sınıflandırılması ve farklı algoritmaların performanslarının karşılaştırılması amaçlanmıştır.

## Kullanılan Yöntemler ve Algoritmalar
- **Veri Ön İşleme:** `LabelEncoder` ile kategorik verilerin sayısal kodlanması.
- **Veri Bölme:** Tabakalı Örnekleme (**Stratified Sampling**) yöntemiyle %80 Eğitim (Train), %20 Test kümesi ayrımı.
- **Modeller:**
  - Karar Ağaçları (Decision Tree)
  - Rasgele Ormanlar (Random Forest)
  - Naïve Bayes (CategoricalNB)
  - K-En Yakın Komşu (K-Nearest Neighbors - KNN)
- **Değerlendirme:** Confusion Matrix (Karmaşıklık Matrisi), Accuracy, Precision, Recall ve F1-Score metrikleri.

## Performans Sonuçları (Result Tablosu)

| Model | Accuracy | F1-score | Precision | Recall |
| :--- | :---: | :---: | :---: | :---: |
| **Karar Ağaçları** | 1.0000 | 1.0000 | 1.0000 | 1.0000 |
| **Rasgele Ormanlar** | 1.0000 | 1.0000 | 1.0000 | 1.0000 |
| **Naive Bayes** | 0.9458 | 0.9410 | 0.9901 | 0.8966 |
| **K-en yakın komşu** | 0.9969 | 0.9968 | 0.9949 | 0.9987 |

## Dosya Yapısı
- `elif_kavak_dm_kod.ipynb`: Tüm analiz, görselleştirme ve model eğitim kodlarının yer aldığı Jupyter Notebook dosyası.
- `elif_kavak_dm_rapor.pdf`: Calibri (10pt) formatında hazırlanmış 3 sayfalık resmi proje raporu.
- `mushrooms.csv`: Analizde kullanılan veri seti.
- `confusion_matrices.png` & `model_comparison.png`: Model değerlendirme ve metrik grafik görselleri.
