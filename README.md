# Review Analysis System

This project analyzes user reviews to determine sentiment (positive, negative, neutral) and classifies data using text mining techniques.  
It leverages **Natural Language Processing (NLP)** and **Machine Learning** methods to extract meaningful insights from review content.

---

## Project Objective

User reviews play a critical role in evaluating products and services today. However, manually analyzing these reviews can be time-consuming.  
This project aims to automate the review analysis process to achieve the following:

- **Sentiment Analysis:** Determines whether a review is **positive**, **negative**, or **neutral**.  
- **Text Preprocessing:** Cleans unnecessary words and characters from reviews for more efficient analysis.  
- **Machine Learning:** Trains models to accurately classify new reviews.  
- **Word Analysis:** Extracts the most frequently used words and expressions.  
- **Visualization:** Presents results with graphs for easier understanding.

---

## Technologies & Libraries Used

This project is developed in **Python** and utilizes the following libraries:

### **Data Processing & NLP:**  
- **`pandas`** → For dataframes and data cleaning.  
- **`numpy`** → For numerical operations and arrays.  
- **`nltk`** → For natural language processing tasks (stopword removal, tokenization, etc.).  
- **`re`** → For cleaning data using regular expressions.  

### **Machine Learning & Model Training:**  
- **`scikit-learn`** → To train and evaluate the sentiment analysis model.  
- **`TF-IDF Vectorizer`** → Converts text into numerical vectors.  
- **`Logistic Regression / Naive Bayes`** → Machine learning classifiers used for review classification.  

### **Visualization:**  
- **`matplotlib`** → For plotting graphs and visualizing analysis results.  
- **`seaborn`** → For more detailed and stylish visualizations.  
- **`wordcloud`** → To display the most frequent words in reviews as a word cloud.

---

## Project Steps

1️ **Data Collection:**  
- User reviews are added in `.csv` format to the **data/** folder.

2️ **Preprocessing:**  
- Cleaning special characters  
- Converting text to lowercase  
- Removing stopwords  
- Lemmatization (reducing words to their root form)  

3️ **Feature Extraction:**  
- Converting text to numerical format using **TF-IDF Vectorization**  

4️ **Training Machine Learning Models:**  
- Models such as **Logistic Regression** and **Naive Bayes** are trained for classification  

5️ **Prediction & Evaluation:**  
- The model is evaluated on test data.  
- Metrics such as **Accuracy, Precision, Recall, F1 Score** are calculated  

6️ **Result Visualization:**  
- Sentiment distribution graphs are created.  
- Word clouds display the most frequently used words.

**Word Cloud:**  
A visualization showing the most common words in the reviews.

**Sample Model Output:**  
| Review                                      | Sentiment |
|--------------------------------------------|-----------|
| "This product is amazing, I recommend it!" | Positive  |
| "The price is too high and the quality is low." | Negative  |
| "The product is okay, but it could be better." | Neutral   |


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



