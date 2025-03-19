# Yorum Analiz Sistemi

Bu proje, kullanıcı yorumlarını analiz ederek duygu durumu (olumlu, olumsuz, nötr) belirleme ve metin madenciliği teknikleriyle verileri sınıflandırma işlemlerini gerçekleştirir. 
**Doğal Dil İşleme (NLP)** ve **Makine Öğrenmesi** yöntemlerini kullanarak yorumların içeriğini anlamlandırmayı amaçlar.  

---

## Proje Amacı  

Günümüzde kullanıcı yorumları, ürün ve hizmet değerlendirmelerinde kritik bir rol oynamaktadır. Ancak bu yorumları manuel olarak incelemek zaman alıcı olabilir. Bu proje, yorumları otomatik olarak analiz ederek aşağıdaki işlemleri gerçekleştirmeyi hedefler:  

- **Duygu Analizi:** Yorumların **olumlu**, **olumsuz** veya **nötr** olduğunu belirler.  
- **Metin Ön İşleme:** Yorumlardan gereksiz kelimeleri ve karakterleri temizleyerek analizi daha verimli hale getirir.  
- **Makine Öğrenmesi:** Model eğitimi yaparak yeni yorumları doğru bir şekilde sınıflandırmayı amaçlar.  
- **Kelime Analizi:** En sık kullanılan kelimeleri ve ifadeleri çıkarır.  
- **Görselleştirme:** Sonuçları grafiklerle destekleyerek daha anlaşılır hale getirir.  

---

## Kullanılan Teknolojiler & Kütüphaneler  

Bu proje, **Python** dilinde geliştirilmiş olup aşağıdaki kütüphaneler kullanılmıştır:  

### **Veri İşleme ve NLP:**  
**`pandas`** → Veri çerçeveleri ve veri temizleme işlemleri için kullanıldı.  
**`numpy`** → Sayısal işlemler ve diziler için kullanıldı.  
**`nltk`** → Doğal dil işleme işlemleri (stopword temizleme, kelime ayrıştırma vb.) için kullanıldı.  
**`re`** → Düzenli ifadeler kullanarak veri temizleme işlemleri gerçekleştirildi.  

### **Makine Öğrenmesi ve Model Eğitimi:**  
**`scikit-learn`** → Duygu analizi modeli eğitmek ve değerlendirmek için kullanıldı.  
**`TF-IDF Vectorizer`** → Yorumları sayısal vektörlere dönüştürmek için kullanıldı.  
**`Logistic Regression / Naive Bayes`** → Yorumları sınıflandırmak için kullanılan makine öğrenmesi modelleri.  

### **Görselleştirme:**  
**`matplotlib`** → Grafikler ve analiz sonuçlarını görselleştirmek için kullanıldı.  
**`seaborn`** → Daha şık ve detaylı görseller oluşturmak için kullanıldı.  
**`wordcloud`** → Yorumlarda en sık geçen kelimeleri kelime bulutu olarak göstermek için kullanıldı.  


## Proje Adımları  

1️ **Veri Toplama:**  
- Kullanıcı yorumları `.csv` formatında **data/** klasörüne eklenir.  

2️ **Ön İşleme:**  
- Özel karakterlerin temizlenmesi  
- Küçük harfe dönüştürme  
- Stopword’lerin (gereksiz kelimelerin) kaldırılması  
- Kelimelerin köklerine indirgenmesi (Lemmatization)  

3️ **Özellik Çıkarma:**  
- **TF-IDF Vektörleştirme** ile metinleri sayısal formata dönüştürme  

4️ **Makine Öğrenmesi Modeli Eğitme:**  
- **Lojistik Regresyon**, **Naive Bayes** gibi sınıflandırıcılar ile eğitim yapılır.  

5️ **Tahmin ve Değerlendirme:**  
- Model, test verisi ile değerlendirilir.  
- **Doğruluk (Accuracy), Hassasiyet (Precision), Duyarlılık (Recall), F1 Skoru** gibi metrikler hesaplanır.  

6️ **Sonuçları Görselleştirme:**  
- Duygu dağılım grafikleri oluşturulur.  
- Kelime bulutu ile en sık kullanılan kelimeler gösterilir.  

**Kelime Bulutu:**  
Yorumlarda en sık kullanılan kelimeleri içeren kelime bulutu (Word Cloud).  

**Örnek Model Çıktısı:**  
| "Bu ürün harika, herkese tavsiye ederim!"  | Olumlu |
| "Fiyatı çok pahalı ve kalitesi düşük."     | Olumsuz |
| "Ürün fena değil ama daha iyi olabilirdi." | Nötr |



