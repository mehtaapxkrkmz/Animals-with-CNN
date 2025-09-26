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
- Optimizasyon Algoritmaları: Adam,RMSProp
- Loss Fonksiyonu: Categorical Crossentropy

## Metrikler ve Değerlendirme

Eğitim ve değerlendirme sürecinde aşağıdaki metrikler kullanılmıştır:
- Accuracy / Loss grafikleri (epoch bazında)
- Confusion Matrix (sınıflar arası başarı)
- Classification Report (Precision, Recall, F1-score)
- Grad-CAM / Heatmap görselleştirmesi (modelin hangi bölgelerden etkilendiğini göstermek için)

##  Ek Çalışmalar

- Random Search hiperparametre optimizasyonu denendi.
- Kaggle GPU ortamında eğitim yapıldı.

## Sonuç

- Bu çalışmada, hayvan görselleri üzerinde bir sınıflandırma modeli geliştirildi.
- GradCAM kısmı için: Notebook hücreleri çalıştırılıp test klasöründen seçilen bir görsel uzantısı kullanılırsa heatmap sonucu görülebilir. Bu sorun çözülemedi, kaggle'da output klasöründe split işlemi sonucunda oluşan test klasöründen görsel seçilmelidir.
- Elde edilen maksimum performansı gösteren model ve performans metrikleri:
- 
  <img width="961" height="422" alt="image" src="https://github.com/user-attachments/assets/bc525a42-a3ad-429b-aff3-118a1294f370" />

  <img width="662" height="552" alt="image" src="https://github.com/user-attachments/assets/835d4010-37de-490c-96d1-276d2686c4d1" />



## Gelecekte Yapılabilecek İyileştirmeler:

- Daha derin CNN veya transfer learning kullanımı
- Modelin Streamlit / Gradio arayüzü ile deploy edilmesi
- Veri setinin büyütülmesi ve augmentasyon teknikleri ile çeşitlendirilmesi

# Kaggle Linki
- [https://www.kaggle.com/code/mehtapkorkmaz/animals-with-cnn](https://www.kaggle.com/code/mehtapkorkmaz/animals-with-cnn)
