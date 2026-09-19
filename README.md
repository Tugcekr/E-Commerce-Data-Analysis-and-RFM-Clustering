# E-Commerce-Data-Analysis-and-RFM-Clustering
# 🛒 E-Commerce Data Analytics & Machine Learning Customer Segmentation

Brezilya merkezli Olist e-ticaret verisi üzerinde uçtan uca veri analitiği, istatistiksel hipotez testleri ve makine öğrenmesi uygulamaları içeren portfolyo projesidir.

## 🚀 Proje Amacı ve Çıktılar
Bu projenin amacı, kargo teslimat ağındaki operasyonel darboğazları tespit etmek ve müşterileri kârlılıklarına göre gruplandırarak pazarlama stratejileri geliştirmektir. 
* **İstatistiksel A/B Testi (ANOVA & Ki-Kare):** Hacimli ürünlerin standart kargo ağında istatistiksel olarak anlamlı seviyede gecikme yarattığı kanıtlanmıştır.
* **Makine Öğrenmesi (K-Means):** Müşterilerin %97'sinin tek seferlik alışveriş yapması nedeniyle çöken kural tabanlı RFM modeli yerine, K-Means gözetimsiz öğrenme algoritması kullanılmış ve optimum 4 doğal küme (VIP, Yeni, Riskli, Kayıp) tespit edilmiştir (Silhouette Score doğrulaması yapılmıştır).
* **İş Zekası:** Çıkarılan 2600 kişilik "VIP Müşteri Listesi" pazarlama departmanı için Excel'e aktarılmış ve yönetici kararları için Power BI paneli tasarlanmıştır.

## 🛠️ Kullanılan Teknolojiler
* **Veritabanı & ETL:** PostgreSQL (SQL JOIN, Group By, Aggregation)
* **Veri Bilimi & İstatistik:** Python (Pandas, SciPy, Scikit-Learn, K-Means Clustering)
* **İş Zekası & Veri Görselleştirme:** Power BI (DAX, Interactive Dashboards, Map Visuals)

## 📊 Power BI Yönetici Paneli (Dashboard)
Aşağıda operasyon ve pazarlama ekipleri için tasarlanan interaktif panelin bir görüntüsü yer almaktadır:

## 💼 Stratejik İş Aksiyonları
1. **Lojistik:** Yüksek maliyetli kargolar hızlı teslim edilirken, orta segment ücretlerde (25-75 BRL) 60 güne varan gecikmeler tespit edilmiştir. Sorun mesafede değil, standart kargo ağının kapasitesindedir. RJ ve BA eyaletlerine "fulfillment center" (bölgesel depo) açılması önerilmiştir.
2. **CRM & Pazarlama:** Toplam cironun çok büyük bir kısmını oluşturan Küme 2 (VIP/Balinalar) segmentine yönelik özel "sadakat programı" tasarlanmalı ve doğrudan bu kitleye kampanya çıkılmalıdır.
3. Ham CSV verileri, güvenlik standartlarına uygun şekilde (environment variables kullanılarak) Python SQLAlchemy ve Psycopg2 kütüphaneleri ile yerel PostgreSQL veritabanına aktarılarak (ETL süreci) analitik bir Veri Mart'ı inşa edilmiştir.
