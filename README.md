# 🎯 BETS PROJECT – Spor Bahislerinde Kullanıcı Segmentasyonu

Bu proje, spor bahislerinde kullanıcıların davranışsal örüntülerini analiz ederek **anlamlı müşteri segmentleri** oluşturmayı amaçlar. Kullanıcıların bahis sıklığı, risk düzeyi, tercih ettiği sporlar, kazanç-kayıp dinamikleri ve oran davranışları incelenerek K-means tabanlı bir segmentasyon modeli geliştirilmiştir.

---

## 📁 İçerik Başlıkları
- Veri seti ve değişkenlerin açıklaması  
- Veri temizleme & ön işleme  
- Özellik mühendisliği (stake, gain, GGR, spor oranları vb.)  
- Normalize edilmiş değişkenlerle K-means segmentasyonu  
- Küme sayısı seçimi (Elbow, Silhouette, Davies-Bouldin karşılaştırması)  
- PCA / t-SNE ile görsel analiz  
- Segment yorumlama & iş çıktıları

---

## 📘 Notebook
Tüm analizler aşağıdaki notebook içinde sunulmaktadır:

👉 **`bets_profilling.ipynb`**

---
🧠 Kullanılan Yöntemler
✔️ 1) Veri Ön İşleme

Eksik veri kontrolü

Aykırı değer incelemesi

Standartlaştırma (StandardScaler)

Oran değişkenleri: single/multiple ratio, sport ratios

✔️ 2) Özellik Mühendisliği

Kullanıcı bazlı özet değişkenler (mean stake, total gain, GGR, win rate, odds istatistikleri)

Spor bazlı sayma / oran değişkenleri

Davranışsal pattern çıkarımı

✔️ 3) Kümeleme

K-means

En uygun küme sayısı için çoklu metrik karşılaştırması

İş mantığı ile segmentlerin yorumlanması

Örneğin: yüksek stake – düşük kazanç, bonus avcısı, düşük riskli oyuncu gibi davranış profilleri

✔️ 4) Görselleştirme

PCA bileşenleri ile 2-boyutlu segment haritası

t-SNE ile yüksek boyutlu yapının görselleştirilmesi

Segment bazlı dağılımlar & istatistiksel özetler

🚀 Nasıl Çalıştırılır?
1) Gerekli kütüphaneler
pip install pandas numpy scikit-learn matplotlib seaborn

2) Notebook’ı açın
jupyter notebook bets_profilling.ipynb

📌 İş Çıktısı Ne Sağlar?

Bu segmentasyon modeli ile:

Riskli kullanıcı davranışları erken tespit edilebilir

Bonus stratejileri kullanıcı tiplerine göre optimize edilebilir

LTV (life-time value) tahminlerindeki doğruluk artırılabilir

Kampanya / kişiselleştirme modelleri güçlendirilebilir

Fraud veya sıra dışı davranış örüntüleri daha hızlı yakalanabilir

👩‍💻 **Geliştirici**

**Aydan Aloğlu**

**Büyük Veri Analitiği • Python • Power BI**
