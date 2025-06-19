## !!! EKLENMESİ GEREKENLER 
* APİ VERİ ÇEKİLMELİ
* 






# 🧠 Kişisel Proje Notlarım
Bu dosya, bu projeyi geliştirirken öğrendiğim yeni kavramları, yaşadığım problemleri ve çözümleri belgelemek için oluşturulmuştur. Hem kendi gelişimimi takip etmek hem de başkalarının faydalanması amacıyla paylaşıyorum.

---

## 🚀 Proje Amacı

Bu proje, bulut tabanlı bir makine öğrenimi pipeline’ı oluşturmayı hedefliyor. Amaç; veri çekme, işleme, model eğitimi, değerlendirme ve otomatik yeniden eğitme süreçlerini bir araya getiren uçtan uca bir sistem kurmak.

---

## 📚 Öğrendiğim Yeni Kavramlar

SımpleImputer ==> Eksik verileri doldurur
*mean --> ortalamayla doldurur
*median --> ortanca değerle doldurur
*most_frequent --> en sık tekrar eden değerler doldurur


sklearn.compose ==> ColumnTransformer sınıfı ile bilinir
 * Numeric kategoriler -- StandardScaler ile 
 * Categoryc -- OneHotEncoder ile 
 * Text kolonlar-- TfidVectorized 





numeric_transformer = StandartScaler()
oh_transformer = OneHotEncoder()


from dataclasses import dataclass 

daha temiz bir class yapısı oluşturur. __init__ otomatik olarak gelir. 












------------------------------------------------------------------------------
## Kernel Distribution Function: Çekirdek Dağılım Fonksiyonu, bir veri setindeki her bir veri noktası etrafında bir çekirdek fonksiyonu (kernel function) yerleştirerek ve bu çekirdekleri toplayarak yoğunluk tahminini oluşturur. Matematiksel olarak, bir veri seti $ \{x_1, x_2, \dots, x_n\} $ için çekirdek yoğunluk tahmini şu şekilde ifade edilir:

![alt text](image.png)
------------------------------------------------------------------------------
## mean imputatiton: 
  eksik veri var ise --> df.isna().sum()
  o sütunun ortalaması alınıp doldurulur avantaj ve dezavantajları vardır.

  `_,_, exc_tb = error_detail.exc_info() `  -->  exc_info() 3 ögeli bir lisdte döndürüyor burdada sonuncu elemanı alıyoruz _,_, diyerek

  ## def __init__(self, ....): 
  Bu sınıftan yeni bir nesne oluşturulduğunda (instance) otomatik olarak çağırılır.
  Nesneye ait başlangıç verilerini tanımlamak için kullanılır
  
  class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age,

   ## def __str__(self): 
   Nesneyi ekrana açıklanabilir şekilde yazdırmaya yarar. Örneğin p = Person("Ayşe" , 25)
   print(p) olarak yazdırdığımız zaman terminalde --> Ayşe is 25 years old yazısını alabiliriz.

       def __str__(self):
        return f"{self.name} is {self.age} years old."




















## ⚠️ Karşılaştığım Problemler ve Çözümler

### ✅ `exc_tb = sys.exc_info()[2]` ne işe yarıyor?
**Problem:** Hata mesajlarında hangi dosyada ve satırda hata olduğunu göstermek istiyordum.

**Çözüm:**

