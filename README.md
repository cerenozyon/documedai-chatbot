🧠 DocuMed AI Bot
🔍 Proje Amacı
DocuMed AI Bot, Retrieval-Augmented Generation (RAG) mimarisi kullanılarak geliştirilmiş bir sağlık teknolojisi sohbet botudur. Amaç, hastabaşı monitörlerin kullanım kılavuzlarından bilgi çekerek, sağlık personeli veya teknisyenlerin cihazlarla ilgili sorularına hızlı, doğru ve güvenilir yanıtlar verebilen bir yapay zekâ destekli asistan oluşturmaktır.
Bu sistem, tıbbi cihaz dokümantasyonuna erişimi kolaylaştırarak zaman tasarrufu, hataların azaltılması ve eğitim süreçlerinin desteklenmesi hedeflerini taşır.

🗂️ Veri Seti Hakkında Bilgi
Projede, Türkiye’deki hastanelerde yaygın olarak kullanılan GE, Philips, Mindray gibi markalara ait hastabaşı monitörlerin halka açık kullanım kılavuzları kullanılmıştır.
Bu dokümanlarda yer alan bilgiler:
* Cihaz kurulumu ve bağlantı talimatları
* Temel fonksiyonlar ve ekran menüleri
* Hasta bağlantı prosedürleri
* Bakım, kalibrasyon ve hata giderme adımları
* Uyarı ve alarm mesajları
Veri ön işleme aşamasında PDF dosyalar metne dönüştürülmüş, bölümler halinde ayrıştırılmış ve embedding modeline uygun şekilde vektörleştirilmiştir.

⚙️ Kullanılan Yöntemler
🧩 1. RAG (Retrieval-Augmented Generation) Mimarisi
Projede, RAG pipeline yaklaşımı ile bilgi çekme (retrieval) ve cevap üretimi (generation) süreçleri entegre edilmiştir.
Kullanılan temel bileşenler:
Bileşen	Kullanılan Teknoloji / Alternatif
Framework	LangChain veya Haystack
LLM (Generation Model)	OpenAI API, Gemini API veya Hugging Face LLM’leri
Embedding Model	Google, Cohere veya SentenceTransformers tabanlı model
Vektör Veritabanı	Chroma, FAISS veya Pinecone
Frontend	Streamlit / Gradio tabanlı web arayüzü
💻 Kodun Çalışma Kılavuzu
1️⃣ Ortam Kurulumu
git clone https://github.com/kullaniciadi/DocuMed-AI-Bot.git
cd DocuMed-AI-Bot
2️⃣ Sanal Ortam Oluşturma
python -m venv venv
source venv/bin/activate  # Windows için: venv\Scripts\activate
3️⃣ Gerekli Kütüphanelerin Kurulumu
pip install -r requirements.txt
4️⃣ Uygulamayı Çalıştırma
streamlit run app.py
veya
python app.py
Tarayıcıda http://localhost:8501 adresine giderek web arayüzünü görüntüleyebilirsiniz.

🧠 Çözüm Mimarisi
DocuMed AI Bot, 3 katmandan oluşur:
1. Veri Katmanı – Kullanım kılavuzlarının metin temsilleri embedding olarak saklanır.
2. Bilgi Getirme Katmanı – Kullanıcının sorgusuna en yakın doküman parçalarını FAISS/Chroma üzerinden getirir.
3. Cevap Üretme Katmanı – Getirilen bilgiler LLM’e verilerek doğal dilde yanıt oluşturulur.
Bu yapı, büyük dil modellerinin genel bilgiye dayalı “halüsinasyon” eğilimini azaltır ve doğrudan kılavuz içeriğine dayalı yanıtlar sağlar.

🌐 Web Arayüzü & Ürün Kılavuzu
Botun web arayüzü, kullanıcı dostu bir tasarımla sunulmuştur. Kullanıcı, metin kutusuna “Cihaz nasıl kalibre edilir?” gibi bir soru girdiğinde sistem:
1. Sorguya uygun metin parçalarını veri tabanından getirir.
2. LLM ile doğal bir yanıt oluşturur.
3. Cevabı ve kaynak doküman bölümünü birlikte görüntüler.
🔗 Canlı Demo Linki: https://documed-ai.streamlit.app (proje deploy edildiğinde güncellenecek)

📊 Elde Edilen Sonuçlar
Proje şu anda geliştirme aşamasındadır. Tamamlandığında burada, botun doğruluk oranı, kullanıcı deneyimi geri bildirimleri ve örnek etkileşim ekranları paylaşılacaktır.

🧾 Kaynaklar
* Gemini API Docs
* Haystack Documentation
* Hugging Face Datasets
* Chatbot Deploy Template

👩‍💻 Katkıda Bulunanlar
* Proje Geliştiricisi: [Adınız]
* Bootcamp: Akbank GenAI Bootcamp – Yeni Nesil Proje Kampı
* Tarih: Ekim 2025
