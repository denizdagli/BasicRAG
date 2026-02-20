# 🤖 Basic RAG (Retrieval-Augmented Generation) Assistant
Bu proje, LangChain ve OpenAI kullanarak belirli bir web sayfasındaki (Lilian Weng - LLM Powered Autonomous Agents) bilgileri analiz eden ve bu bilgilere dayanarak soruları yanıtlayan temel bir RAG (Artırılmış Bilgi Geri Getirimi) uygulamasıdır.

## 🚀 Özellikler
- Web Scraping: WebBaseLoader ve BeautifulSoup ile hedeflenmiş içerik çekme.

- Akıllı Metin Bölme: Uzun makaleleri anlamlı parçalara (chunks) ayıran RecursiveCharacterTextSplitter.

- Vektör Veritabanı: Hızlı ve yerel veri depolama için ChromaDB entegrasyonu.

- Streaming Output: Yanıtları gerçek zamanlı (kelime kelime) akış şeklinde görüntüleme.

- Modern LCEL: LangChain Expression Language kullanılarak oluşturulmuş optimize zincir yapısı.

## 🛠️ Kullanılan Teknolojiler
- Framework: LangChain

- LLM: OpenAI GPT-3.5-Turbo

- Embeddings: OpenAI Embeddings

- Vector Store: ChromaDB

- Environment: Python 3.11+

## 📦 Kurulum
1 - Depoyu klonlayın:
    `git clone https://github.com/denizdagli/BasicRAG.git
    cd BasicRAG`

2 - Sanal ortam oluşturun ve aktif edin:
    `python -m venv venv
        source venv/bin/activate  # Windows için: venv\Scripts\activate`

3 - Gerekli kütüphaneleri yükleyin:
    `pip install langchain langchain-openai langchain-chroma langchain-community beautifulsoup4 python-dotenv`

4 - .env dosyasını oluşturun:
Proje dizinine .env dosyası ekleyin ve OpenAI API anahtarınızı girin:

    `OPENAI_API_KEY=your_api_key_here`


## 📋 Kullanım
Sistemi çalıştırmak ve makale hakkında soru sormak için:
`python main.py`

## 📝 Örnek Çıktı
Soru: "What is the main idea of the article?" Cevap: "The main idea of the article is to discuss the challenges and performance evaluation of LLM-centered agents, focusing on resource management..."

