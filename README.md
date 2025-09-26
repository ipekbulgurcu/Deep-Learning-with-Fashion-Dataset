# 🌟 Derin Öğrenme ile Giyim Görüntüsü Sınıflandırması: Kategori Sayılarının Performansa Etkisi

## 📖 Proje Hakkında

Bu depo, Derin Öğrenme (Deep Learning) yöntemlerini kullanarak gerçek dünya giyim ürünlerinin görüntü sınıflandırmasını (Image Classification) incelemeyi amaçlamaktadır. Projenin ana hedefi, aynı temel **Evrişimli Sinir Ağı (CNN)** mimarisi kullanıldığında, sınıflandırma modelinin performansının **kategori sayısına bağlı olarak nasıl değiştiğini** uygulamalı olarak gözlemlemektir.

İki ana senaryo üzerinde karşılaştırma yapılmıştır:
1.  **5 Sınıflı Genel Sınıflandırma** (Daha az sınıf, daha basit bir problem).
2.  **20 Sınıflı Detaylı Sınıflandırma** (Daha çok sınıf, daha karmaşık ve zorlu bir problem).

---

## 🖼️ Veri Kümesi (Dataset)

Bu projede kullanılan veri kümesi, giyim ürünleri alanındaki popüler bir Kaggle kaynağıdır.

### Veri Kümesi Bilgisi

| Özellik | Değer |
| :--- | :--- |
| **Veri Seti Adı** | Fashion Product Images (Small) |
| **Orijinal Kategori Sayısı** | ~45+ çeşit detaylı giyim ürünü |
| **Kullanım Amacı** | Orijinal veriden **5** ve **20** kategorilik alt kümeler oluşturarak farklı zorluk seviyelerinde modelleri eğitmek. |

### 🔗 Kaggle Kaynağı

> 🚨 **Lütfen Buraya Kaggle Linkini Ekleyin:**
>
> **[Fashion Product Images (Small) - Kaggle]** (https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small)

---

## 📂 Dosyalar ve Model Karşılaştırması

Bu depoda, her biri farklı bir sınıflandırma zorluğunu ele alan iki ana Jupyter Notebook dosyası bulunmaktadır:

### 1. `fashion-dataset-5-categories.ipynb`

Bu senaryo, giyim ürünlerini **5 ana kategoriye** (Örn: Üst Giyim, Alt Giyim, Ayakkabı, Aksesuar, vb.) indirgeyerek daha genel bir sınıflandırma problemi oluşturur.

| Özet Bilgi | Değer |
| :--- | :--- |
| **Sınıf Sayısı** | **5** |
| **Sınıflandırma Tipi** | Genel |
| **Model Mimarisi** | Evrişimli Sinir Ağı (CNN) |
--
https://www.kaggle.com/code/pekbulgurcu/fashion-dataset-5-categories
---
### 2. `fashion-dataset-20-categories.ipynb`

Bu senaryo, veri setindeki en sık kullanılan ve ayrışabilen **20 farklı giyim türünü** (Örn: T-shirt, Saree, Jeans, Dress, vb.) kullanarak daha detaylı bir sınıflandırma problemi oluşturur.

| Özet Bilgi | Değer |
| :--- | :--- |
| **Sınıf Sayısı** | **20** |
| **Sınıflandırma Tipi** | Detaylı |
| **Model Mimarisi** | Evrişimli Sinir Ağı (CNN) |
--
https://www.kaggle.com/code/pekbulgurcu/fashion-dataset-20-categories
---

## ⚙️ Kullanılan Teknolojiler

| Alan | Kütüphane Adı | Amaç |
| :--- | :--- | :--- |
| **Derin Öğrenme** | `TensorFlow` / `Keras` | CNN modelini tanımlama, eğitme ve değerlendirme. |
| **Veri Manipülasyonu** | `NumPy`, `Pandas` | Görüntü dizilerini işleme ve veri setinin meta verilerini (`styles.csv`) okuma. |
| **Veri Görselleştirme** | `Matplotlib` / `Seaborn` | Eğitim geçmişi ve sonuçları grafikleme. |
| **Veri İndirme** | `kaggle` | Veri setini doğrudan indirme (Kurulum adımına bakınız). |

---
## Linkler
https://www.kaggle.com/pekbulgurcu
https://www.kaggle.com/code/pekbulgurcu/fashion-dataset-5-categories
https://www.kaggle.com/code/pekbulgurcu/fashion-dataset-20-categorie
---

## 🚀 Kurulum ve Çalıştırma Rehberi

Projeyi kendi ortamınızda çalıştırabilmek için **Kaggle API** üzerinden veri kümesini indirmeniz gerekmektedir.

### 1. Önkoşullar

* Python 3.x sürümü
* **Kaggle API Anahtarı:** Kaggle hesabınızdan indirdiğiniz `kaggle.json` dosyasını sisteminizde yapılandırın.

### 2. Bağımlılıkları Yükleme

Gerekli tüm kütüphaneleri yükleyin:

```bash
pip install tensorflow keras numpy pandas scikit-learn jupyter matplotlib seaborn kaggle
