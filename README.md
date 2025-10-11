
# 🧠 DocuMed AI Bot

**DocuMed AI Bot**, RAG (Retrieval-Augmented Generation) mimarisi kullanılarak geliştirilmiş, **tıbbi cihaz kullanım kılavuzlarına odaklanan bir yapay zeka sohbet botudur**.  
Bu bot, kullanıcıların tıbbi cihazlarla ilgili sorduğu sorulara **ilgili dokümanlardan alıntılar yaparak** yanıt verir ve tıbbi bilgilere erişimi kolaylaştırmayı hedefler.

---

## 🚀 Proje Adımları

### 1. Geliştirme Ortamı (GitHub & README.md)
Projenin tüm kodları bu GitHub reposunda bulunmaktadır.  
README.md dosyası, projenin genel yapısını, amacını ve nasıl çalıştırılacağını açıklamaktadır.

### 2. Veri Seti Hazırlama
Botun bilgi tabanı, çeşitli **tıbbi cihazların halka açık kullanım ve servis kılavuzlarından** oluşturulmuştur.  
Bu dokümanlar, RAG pipeline’ı için temel bilgi kaynağı olarak kullanılır.  
Örnek cihazlar:
- EKG cihazı  
- Kan basıncı monitörü  
- Oksijen konsantratörü  
- Hasta monitörü  

### 3. Kodun Çalışma Kılavuzu
Projeyi yerelde veya sunucuda çalıştırmak için gereken adımlar aşağıda detaylandırılacaktır.  
🔹 *To be updated...*

### 4. Çözüm Mimarisi
Projede kullanılan RAG mimarisi aşağıdaki ana bileşenlerden oluşur:
- **Retriever:** Bilgi tabanından en alakalı doküman parçalarını getirir.  
- **Generator:** Model, bu bilgileri kullanarak kullanıcı sorusuna yanıt üretir.  
- **Pipeline:** Kullanıcı sorgusu → Embedding → Retrieval → Generation adımlarını zincirler.

### 5. Web Arayüzü & Ürün Kılavuzu
Botun web arayüzü kullanıcı dostu bir sohbet ekranı sunar.  
Kullanıcılar tıbbi cihazlarla ilgili sorularını buradan iletebilir.  
🔹 *Demo linki eklenecektir.*

---

## 📂 Veri Seti Hakkında Bilgi

Projede, tıbbi cihaz üreticilerinin web sitelerinden elde edilen halka açık kullanım kılavuzları kullanılmıştır.  
Bu kılavuzlar aşağıdaki bilgileri içerir:
- Teknik özellikler  
- Kullanım talimatları  
- Sorun giderme adımları  
- Güvenlik uyarıları  

> Veri setinin amacı, botun tıbbi cihazlarla ilgili spesifik sorulara **doğru, açıklayıcı ve güvenilir yanıtlar** vermesini sağlamaktır.

---

## 🧩 Kullanılan Yöntemler ve Teknolojiler

### 🔹 RAG Pipeline Framework
Projede **LangChain** veya **Haystack** framework’ü kullanılacaktır.

### 🔹 Generation Model
Yanıt üretimi için:
- [ ] Gemini API  
- [ ] OpenAI API (ör. GPT-4/5)  
- [ ] Hugging Face modellerinden biri  

### 🔹 Embedding Model
Metinleri vektörlere dönüştürmek için:
- [ ] Google Embeddings  
- [ ] Cohere  
- [ ] Sentence Transformers  

### 🔹 Vektör Veritabanı
Vektörlerin depolanması ve hızlı aranması için:
- [ ] Chroma  
- [ ] FAISS  
- [ ] Pinecone  

---

## 📊 Elde Edilen Sonuçlar
🔹 *Bu bölüm proje tamamlandığında doldurulacaktır.*

---

## 🌐 Web Linki
🔹 *Projenin canlı sürümü yayınlandığında bağlantı buraya eklenecektir.*

---

## 👩‍💻 Geliştirici
**Ceren Özyön**  
🎓 Biyomedikal Mühendisliği

📍 İzmir Katip Çelebi Üniversitesi

📫 ceren.czn78@gmail.com


---

## 📜 Lisans
🔹 *Lisans türü belirlendiğinde buraya eklenecektir.*  
*(Örneğin: MIT License)*

---

## 💬 Notlar
- Proje, yalnızca **eğitim ve araştırma amaçlıdır**.  
- Üretilen yanıtlar **profesyonel tıbbi tavsiye yerine geçmez**.
