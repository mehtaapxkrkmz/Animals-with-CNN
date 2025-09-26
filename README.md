# Animal Image Classification with CNN

Bu repo, Global AI Hub Deep Learning Bootcamp kapsamında gerçekleştirilen proje için hazırlanmıştır. Proje, farklı hayvan türlerini içeren görsel veri seti üzerinde derin öğrenme tabanlı sınıflandırma çalışması yapmaktadır.

## Veri Seti
- Seçilen Veri Seti: https://www.kaggle.com/datasets/alessiocorrado99/animals10
- İçerik: 10 farklı hayvan sınıfı (kedi, köpek, at, inek, kuş, tavşan, fare, fil, ayı, kaplumbağa)
- Toplam Görsel Sayısı: ~14.000
- Görseller train,validation ve test setlerine ayrılmıştır.

## Kullanılan Yöntemler ve Algoritmalar
- Convolutional Neural Networks (CNN)
- Hiperparametre Optimizasyonu: Keras Tuner ile filtre sayısı, katman sayısı, öğrenme oranı, dropout oranı gibi parametreler optimize edilmiştir.
- Aktivasyon Fonksiyonu: ReLU (ara katmanlar), Softmax (çıktı katmanı)
- Optimizasyon Algoritmaları: Adam
- Loss Fonksiyonu: Categorical Crossentropy

## Metrikler ve Değerlendirme

Eğitim ve değerlendirme sürecinde aşağıdaki metrikler kullanılmıştır:
- Accuracy / Loss grafikleri (epoch bazında)
- Confusion Matrix (sınıflar arası başarı)
- Classification Report (Precision, Recall, F1-score)
- Grad-CAM / Heatmap görselleştirmesi (modelin hangi bölgelerden etkilendiğini göstermek için)

##  Ek Çalışmalar

- Random Search hiperparametre optimizasyonu ile model performansı artırıldı.
- Kaggle GPU ortamında eğitim yapıldı.

## Sonuç

- Bu çalışmada, hayvan görselleri üzerinde bir sınıflandırma modeli geliştirildi.
- Modeli birkaç kez eğitildi; herhangi bir parametre değiştirilmemesine rağmen accuracy, f1-score gibi metrikler son kaggle notebookta önceki değerlere göre daha düşüktür.Notebook'un önceki versiyonlarından kontrol edilebilir. Burası tekrar optimize edilemedi çünkü hiperparametre optimizasyonun uzun sürüyor olması limit problemi yaratacaktı. Elde edilen maksimum performans metrikleri:
  
<img width="1115" height="472" alt="image" src="https://github.com/user-attachments/assets/a20cabac-6d6f-4fb9-b5f0-a13d7bef2db2" />

<img width="746" height="622" alt="image" src="https://github.com/user-attachments/assets/58292fac-0411-4c3d-859c-38b89065b16f" />



## Gelecekte Yapılabilecek İyileştirmeler:

- Daha derin CNN veya transfer learning kullanımı
- Modelin Streamlit / Gradio arayüzü ile deploy edilmesi
- Veri setinin büyütülmesi ve augmentasyon teknikleri ile çeşitlendirilmesi

# Kaggle Linki
- https://www.kaggle.com/code/mehtapkorkmaz/animals-with-cnn
