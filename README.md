# 🌱 Akıllı Sera Otomasyon Sistemi (Advanced OOP Project)

Bu proje, **İleri Nesne Tabanlı Programlama** dersi kapsamında geliştirilen; bitki türlerinin gereksinimlerine göre sensör verilerini analiz edip aktüatörleri (fan, sulama, ışık vb.) otomatik yöneten kapsamlı bir masaüstü otomasyon yazılımıdır.

## 🚀 Proje Hakkında
Projenin temel amacı, klasik otomasyon mantığını **Solid OOP (Nesne Yönelimli Programlama)** prensipleriyle birleştirerek modüler, genişletilebilir ve sürdürülebilir bir mimari kurmaktır. Veriler **SQLite** veritabanında tutulmakta ve **LINQ** sorguları ile işlenmektedir.

### 🛠️ Kullanılan Teknolojiler ve Mimari
* **Diller & Framework:** C# (.NET 8.0), Windows Forms
* **Veritabanı:** SQLite (CRUD İşlemleri)
* **Mimari:** OOP (Object Oriented Programming), Katmanlı Yapı

## 💻 Teknik Özellikler ve OOP Uygulamaları
Bu projede C# dilinin ileri seviye özellikleri aktif olarak kullanılmıştır:

* **Interface Inheritance:** Modüller arası bağımlılığı yönetmek için Interface'lerin miras alınması (Interface Segregation).
* **Abstract Classes & Overriding:** `Sensor` ve `Aktuator` gibi temel sınıflar soyutlanarak (`abstract`), `SicaklikSensoru` veya `SulamaVanasi` gibi türetilmiş sınıflarda metotlar ezilmiştir (`override`).
* **Polymorphism & Overloading:** Sensör ve aktüatörlerin farklı parametrelerle dinamik olarak oluşturulması (Constructor & Method Overloading).
* **LINQ & Generic Collections:** Sensör verilerinin filtrelenmesi ve listelenmesi için `List<T>`, `Dictionary<K,V>` ve LINQ sorguları kullanılmıştır.
* **Custom Exception Handling:** Hata yönetimi için sisteme özel `SeraException` sınıfı yazılmıştır.
* **Nested Classes & Static Members:** Kontrol mekanizmalarında statik metotlar ve dahili sınıflar kullanılmıştır.

## ⚙️ Modüller
1.  **Bitki ve Bölge Yönetimi:** Bitkilerin su, ışık ve nem gereksinimlerinin tanımlanması.
2.  **Sensör Yönetimi:** Sıcaklık, Nem ve Işık sensörlerinin simülasyonu ve veri okuma.
3.  **Aktüatör Yönetimi:** Fan, Isıtıcı, Lamba ve Sulama vanalarının tetiklenmesi.
4.  **Otomasyon Kontrolcüsü:** Sensör verilerini eşik değerlerle karşılaştırıp karar veren algoritma.

---
**Geliştirici:** Burak Çetinkaya
