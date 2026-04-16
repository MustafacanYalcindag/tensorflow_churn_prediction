# 📊 TensorFlow Müşteri Kaybı (Churn) Tahmini

Bu depo, bir şirketin müşterilerinin ayrılıp ayrılmayacağını (churn) önceden tahmin etmek için tasarlanmış bir **Derin Öğrenme** projesini içermektedir.

## 🎯 Proje Amacı
Projenin temel amacı, müşteri davranışlarını analiz ederek potansiyel kayıpları önceden tespit eden bir sınıflandırma modeli oluşturmaktır.

## 🧠 Model Özellikleri ve Teknolojiler
Proje kapsamında aşağıdaki TensorFlow ve makine öğrenmesi kavramları uygulanmıştır:
* **Framework:** TensorFlow & Keras.
* **Model Tipi:** Çok Katmanlı Yapay Sinir Ağları (Sequential ANN).
* **Aktivasyon Fonksiyonları:** * `ReLU`: Gizli katmanlarda hızlı ve etkili öğrenme için kullanıldı.
    * `Sigmoid`: Çıktı katmanında 0-1 arası olasılık üretmek (Binary Classification) için kullanıldı.
* **Derleme Parametreleri:**
    * `Adam`: Ağırlık optimizasyonu için.
    * `Binary Crossentropy`: Kayıp (loss) fonksiyonu olarak.

## 📊 Veri Seti Yapısı
Veri seti sentetik olarak NumPy ile üretilmiştir ve şu özellikleri içerir:
* **Yaş:** Müşterinin yaşı.
* **Aylık Harcama:** Müşterinin harcama miktarı.
* **Abone Süresi:** Şirkette kalınan ay sayısı.
* **Destek Talebi:** Müşteri hizmetlerine ulaşılan sayı.

Veriler; %70 Eğitim, %15 Doğrulama ve %15 Test olarak bölünmüştür.

## 🛠 Kurulum ve Kullanım

1. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install tensorflow numpy
