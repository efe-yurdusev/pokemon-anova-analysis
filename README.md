# Pokémon Veri Seti Üzerinde ANOVA (F Testi) Analizi

Bu projede Pokémon veri seti kullanılarak, yakalanma oranları (*capture_rate*) ile kategorik değişkenler arasındaki ilişkiler incelenmiştir.

Çalışmanın amacı, farklı gruplar arasında istatistiksel olarak anlamlı fark olup olmadığını **ANOVA (F testi)** ile analiz etmektir.

---

## 📊 Kullanılan Değişkenler

- **name**: Pokémon ismi  
- **capture_rate**: Yakalanma zorluğunu temsil eden nicel değişken  
- **is_legendary**: Pokémon’un efsanevi olup olmadığını belirten ikili kategorik değişken  
- **color**: Pokémon’un renk kategorisi (çok kategorili değişken)

---

## 🧠 Yöntem

Bu çalışmada aşağıdaki analiz adımları uygulanmıştır:

1. Veri, PokeAPI üzerinden çekilmiştir.  
2. Veri temizliği ve ön inceleme yapılmıştır.  
3. Boxplot grafikleri ile dağılımlar görselleştirilmiştir.  
4. İki ayrı doğrusal model kurulmuştur:  
   - capture_rate ~ is_legendary  
   - capture_rate ~ color  
5. Gruplar arası farkların anlamlılığı ANOVA (F testi) ile test edilmiştir.

---

## 📈 Görselleştirme

- Efsanevi duruma göre yakalanma oranları karşılaştırılmıştır.  
- Renk kategorilerine göre dağılım analiz edilmiştir.  

Boxplot grafikleri kullanılarak gruplar arasındaki farklar görsel olarak incelenmiştir.

---

## 🧪 İstatistiksel Sonuçlar

### A) Efsanevi Duruma Göre Analiz

- **p-değeri: 0.006**
- Sonuç:  
  Efsanevi ve efsanevi olmayan Pokémon’lar arasında **istatistiksel olarak anlamlı fark vardır.**

👉 Efsanevi Pokémon’ların yakalanma oranlarının daha düşük olduğu görülmüştür.

---

### B) Renk Kategorisine Göre Analiz

- **p-değeri: 0.816**
- Sonuç:  
  Renk kategorileri arasında **istatistiksel olarak anlamlı fark bulunmamaktadır.**

👉 Görsel farklılıklar olsa da bu farklar istatistiksel olarak anlamlı değildir.

---

## 📌 Genel Değerlendirme

Bu çalışma sonucunda:

- Efsanevi olma durumu, yakalanma oranı üzerinde anlamlı bir etkiye sahiptir.  
- Renk kategorisi ise anlamlı bir etki göstermemektedir.  

Bu durum, veri analizinde görselleştirmenin tek başına yeterli olmadığını, istatistiksel testlerle desteklenmesi gerektiğini göstermektedir.

---

## 🛠 Kullanılan Teknolojiler

- Python  
- Pandas  
- Matplotlib  
- Statsmodels  
- PokeAPI  

---

## 🚀 Proje Amacı

Bu proje;

- veri çekme (API kullanımı)  
- veri analizi  
- görselleştirme  
- istatistiksel modelleme  

becerilerini geliştirmek amacıyla yapılmıştır.

---

## 👤 Geliştirici

Efe Yurdusev
