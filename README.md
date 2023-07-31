# Starbucks Customer Segmentation

- Bu proje Starbucks şirketine ait verileri içermektedir. Şirket mobil uygulama üzerinden kullanıcılarına teklifler (indirim, reklam, bir alana bir bedava) gönderir. Her teklifin geçerlilik süresi vardır.
- 3 ayrı dosyada veriler tutulmaktadır:
1. portfolio -->  teklif kimliklerini ve her teklifle ilgili meta verileri (süre, tür vb.) içerir
2. profile --> her müşteri için demografik veriler
3. transcript --> işlemler, alınan teklifler, görüntülenen teklifler ve tamamlanan teklifler için kayıtlar
 
- 1. Portfolio Veri Seti:
    - id (string) --> teklif kimliği
    - offer_type (string) --> teklif türü (BOGO, indirim, reklam)
    - difficulty (int) --> bir teklifi tamamlamak için gereken minimum harcama
    - reward (int) --> bir teklifi tamamlamak için verilen ödül
    - duration (int) --> teklifin açık kalacağı süre, gün cinsinden
    - channels --> dize şeklinde listeler (email, web, social...)

- 2. Profile Veri Seti:
    - age (int) --> müşterinin yaşı
    - became_member_on (int) --> müşterinin bir uygulama hesabı oluşturduğu tarih
    - gender (str) --> müşterinin cinsiyeti (m,f,o)
    - id (str) --> müşteri kimliği
    - income (float) --> müşteri geliri

- 3. Transcript Veri Seti:
    - event(str) --> kayıt açıklaması (işlem, alınan teklif, görüntülenen teklif, vb.)
    - id (str) --> müşteri kimliği
    - time (int) --> testin başlangıcından itibaren saat cinsinden zaman.
    - value (dict of strings) --> kayda bağlı olarak bir teklif kimliği veya işlem tutarı
 

Projenin temel adımları:
- Data Preparation
- EDA(Exploratory Data Analysis)
- Future Engineering
- A/ B Test
- Customer Segmentation using RFM Analysis
- Data Visualization
