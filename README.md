# Deep Learning-Based Approach for Detecting Malignant Skin Cancer

<details>
  <summary>🇹🇷 <b>Türkçe metni okumak için tıklayın (Click to read in Turkish)</b></summary>
  <br>

  Bu depo (repository), dermatoskopik görüntüler üzerinden kötü huylu deri kanserinin teşhis edilmesi amacıyla gerçekleştirilen derin öğrenme projesinin akademik raporunu içermektedir. 
  
  **Not:** Bu repoda şu an için yalnızca projenin detaylı analizlerini ve sonuçlarını içeren rapor (PDF) yer almaktadır; kaynak kodlar paylaşılmamıştır.

  ## 📌 Proje Özeti
  Deri kanseri, erken teşhis edilmediğinde ölümcül sonuçlara yol açabilen ciddi bir hastalıktır. Bu çalışmada, yapay zeka ve derin öğrenme teknikleri kullanılarak uzmanlara teşhis sürecinde yardımcı olacak, düşük hesaplama maliyetine sahip ve yüksek doğrulukla çalışan bir karar destek sistemi geliştirilmesi hedeflenmiştir.

  Çalışma kapsamında, önceden eğitilmiş (pre-trained) derin öğrenme mimarileri olan **NASNet**, **MobileNetV2** ve **EfficientNet** kullanılmış ve bu modellerin performansları karşılaştırmalı olarak analiz edilmiştir.

  ## 📊 Veri Seti
  Projede 7 farklı deri lezyonu sınıfını (Aktinik Keratoz, Bazal Hücreli Karsinom, Benign Keratoz Lezyonu, Melanom, Nevüs, Dermatofibroma, Vasküler Lezyonlar) içeren, yaklaşık 10.000 görselden oluşan kapsamlı bir veri seti kullanılmıştır. 

  Başlangıçta sınıflar arasında bulunan homojen olmayan dağılımı (veri dengesizliğini) gidermek amacıyla, rastgele alt örnekleme ve veri artırma (data augmentation) teknikleri uygulanmıştır. Model eğitimlerinde veri setinin %80'i eğitim, %20'si ise test aşaması için ayrılmıştır.

  ## 🚀 Modeller ve Başarım Oranları
  Aşırı öğrenme (overfitting) problemlerini engellemek için veri seti dengeleme ve erken durdurma (early stopping) gibi yöntemler uygulanmış olup, transfer öğrenme yöntemiyle elde edilen sonuçlar şu şekildedir:

  * **MobileNetV2:** Eğitim sürecinde en yüksek başarıyı sergileyen model olmuş ve optimize edilmiş yapısı sayesinde **%94** doğruluk (accuracy) oranına ulaşmıştır.
  * **EfficientNet:** Sınıflandırma görevinde aşırı öğrenmenin önüne geçilerek ince ayar (fine-tuning) süreçleri uygulanmış ve başlangıçta **%75.18** sınıflandırma doğruluğu elde edilmiştir.
  * **NASNet:** İki aşamalı olarak optimize edilen eğitim sürecinin sonucunda **%71** doğruluk oranına ulaşmayı başarmıştır.

  ## 📄 Dosya İçeriği
  * `Medikal_Goruntu_Deri_Kanseri.pdf`: Projenin tüm teknik detaylarını, özellik çıkarımı süreçlerini, modellerin karmaşıklık matrislerini (confusion matrix) ve doğruluk/kayıp (accuracy/loss) grafiklerini içeren detaylı rapor dosyası.

</details>

<br>

This repository contains the academic report of a deep learning project aimed at diagnosing malignant skin cancer from dermoscopic images. 
  
**Note:** Currently, this repository only includes the report (PDF) detailing the project's analysis and results; source codes are not shared.

## 📌 Project Summary
Skin cancer is a serious disease that can lead to fatal consequences if not diagnosed early. This study aims to develop a decision support system with low computational cost and high accuracy using artificial intelligence and deep learning techniques to assist experts in the diagnostic process.

The study utilized pre-trained deep learning architectures, namely **NASNet**, **MobileNetV2**, and **EfficientNet**, and comparatively analyzed their performances.

## 📊 Dataset
The project used a comprehensive dataset consisting of approximately 10,000 images covering 7 different skin lesion classes (Actinic Keratosis, Basal Cell Carcinoma, Benign Keratosis Lesion, Melanoma, Nevus, Dermatofibroma, Vascular Lesions). 

To address the initial heterogeneous distribution (data imbalance) among classes, random undersampling and data augmentation techniques were applied. For model training, 80% of the dataset was reserved for training and 20% for testing.

## 🚀 Models and Success Rates
Methods such as dataset balancing and early stopping were applied to prevent overfitting problems. The results obtained via transfer learning are as follows:

* **MobileNetV2:** Emerged as the most successful model during the training process, achieving a **94%** accuracy rate thanks to its optimized structure.
* **EfficientNet:** Fine-tuning processes were applied by preventing overfitting in the classification task, achieving an initial classification accuracy of **75.18%**.
* **NASNet:** Reached a **71%** accuracy rate as a result of a two-stage optimized training process.

## 📄 File Contents
* `Medikal_Goruntu_Deri_Kanseri.pdf`: A detailed report file containing all technical details of the project, feature extraction processes, confusion matrices of the models, and accuracy/loss graphs.
