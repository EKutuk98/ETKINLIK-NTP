# 🎭 Etkinlik Kayıt Sistemi Something went wrong and we can't process that file try again...maalesef yükleyemiyorum hocam...

Etkinlik organizasyonu, katılımcı yönetimi ve biletleme işlemlerini kapsayan tam donanımlı bir etkinlik platformu. PyQt5 ile geliştirilmiş, SQLite veritabanı destekli, gamification ve gelişmiş analiz özellikleri içermektedir.

**🔐 Giriş Bilgileri:**
- Admin: `admin` / `admin123`
- Organizatör: `organizator` / `organizator123`

## 📸 Ekran Görüntüleri

## 📋 Özellikler

### 🏠 Dashboard

- Toplam etkinlik, katılımcı, yaklaşan etkinlik (7 gün) ve toplam gelir KPI kartları
- Sertifika sayısı ve bekleme listesi KPI kartları
- QPainter bar ve pasta grafikler (etkinlik türü, kayıt trendi)
- Son aktiviteler feed


---

### 🎭 Etkinlikler

- Etkinlik ekleme, düzenleme, soft-delete
- Ad, kategori, tarih, kapasite, konum, ücret, açıklama
- Etkinlik durumu (Planlandı / Aktif / Tamamlandı / İptal)
- Anlık arama ve kategori filtresi



---

### 👥 Katılımcılar

- Katılımcı ekleme, düzenleme, soft-delete
- Ad, soyad, email, telefon, şehir, yaş, cinsiyet bilgileri
- Email benzersizlik kontrolü
- Anlık arama



---

### 🎫 Kayıtlar (Bilet İşlemleri)

- Etkinliğe katılımcı kayıt oluşturma
- Bilet tipi seçimi ve ücret hesaplama
- Kayıt durumu: Aktif / İptal / Tamamlandı
- Kapasite doluluk kontrolü
- Anlık arama ve etkinlik filtresi


---

### ⏳ Bekleme Listesi

- Kapasitesi dolan etkinlikler için bekleme listesi
- Sıra numarası ve kayıt tarihi
- Yer açıldığında otomatik bildirim tetikleme
- Bekleme listesinden doğrudan kayıt oluşturma



---

### 📋 Oturumlar

- Etkinlik içi oturum / panel / workshop tanımlama
- Oturum adı, başlangıç-bitiş saati, konum (salon/oda), konuşmacı
- Oturum katılımcı listesi



---

### 🎤 Konuşmacılar

- Konuşmacı ekleme, düzenleme
- Ad, uzmanlık, biyografi, email, telefon
- Konuşmacı bazlı oturum listesi


---

### 💳 Ödemeler

- Kayıt bazlı ödeme takibi
- Ödeme yöntemi (Nakit / Kredi Kartı / EFT / Online)
- Durum: Beklemede / Ödendi / İade
- QPainter ödeme grafiği
- Toplam gelir istatistikleri


---

### 🎟 Bilet Tipleri

- Etkinlik bazlı bilet tipi tanımlama (Normal, VIP, Öğrenci vb.)
- Her tip için fiyat, kontenjan ve açıklama
- Bilet tipi aktif/pasif toggle


---

### 🎓 Sertifikalar

- Tamamlanan etkinlikler için otomatik sertifika oluşturma
- Toplu sertifika oluşturma (etkinlik bazında)
- Katılımcı bazlı sertifika listesi
- Sertifika durumu takibi


---

### 🏅 Gamification

- Katılımcı rozet sistemi (Networker, Öğrenci, Workshop Pro vb.)
- Otomatik rozet kazanma kriterleri
- Katılımcı bazlı rozet ve XP görünümü
- Liderlik tablosu


---

### 📊 İstatistikler

- Kayıt trendi (QPainter Line Chart — son 30 gün)
- Gelir analizi grafiği
- Coğrafi analiz (şehir bazlı katılım dağılımı)
- Demografik analiz (yaş grubu, cinsiyet dağılımı)
- Haftalık yoğunluk


---

### 📢 Bildirimler

- Sistem bildirimleri (yeni kayıt, iptal, kapasite doldu vb.)
- Okunmamış bildirim sayacı
- Tümünü okundu işaretleme


---

### 📝 Anketler

- Etkinlik bazlı anket oluşturma
- Çoktan seçmeli ve açık uçlu sorular
- Katılımcı cevap toplama
- Anket sonuç özeti



---

### 🔬 Gelişmiş Analiz

- Etkinlik karşılaştırma (iki etkinlik yan yana)
- Katılımcı demografik raporu
- Aylık gelir karşılaştırması
- En çok katılım sağlanan etkinlikler



---

### 📄 Şablonlar & Export

- Excel özet raporu (Etkinlikler, Katılımcılar, Ödemeler — 3 sayfalı)
- CSV dışa aktarma
- Etkinlik şablonu kaydetme ve yeniden kullanma


---

### ⚙️ Ayarlar

- Organizasyon adı, email, telefon, logo
- Sertifika şablonu metni
- Hatırlatıcı süresi ayarı
- DB yedekleme



---

### 📋 Aktivite Log

- Tüm işlemlerin kaydı (kim, ne zaman, ne yaptı)
- İşlem türüne göre filtreleme

---

## ❓ Final Soruları

### Sistemde hangi kullanıcılar veya nesneler vardır?

**Kullanıcı Türleri:**
- **Admin** — Tam yetkili; kullanıcı yönetimi, sistem ayarları, tüm modüller
- **Organizatör** — Etkinlik, kayıt, ödeme ve katılımcı yönetimi

**Ana Nesneler / Varlıklar:**
- **Etkinlik** — etkinlik_id, ad, kategori, tarih, kapasite, konum, ücret, durum
- **Katılımcı** — katilimci_id, ad, soyad, email, telefon, şehir, yaş, cinsiyet, durum
- **Kayıt (Bilet)** — kayit_id, etkinlik, katılımcı, bilet tipi, ücret, durum, tarih
- **Bekleme Listesi** — etkinlik, katılımcı, sıra, kayıt tarihi
- **Oturum** — oturum_id, etkinlik, ad, başlangıç, bitiş, konum
- **Konuşmacı** — konusmaci_id, ad, uzmanlık, biyografi, email
- **Ödeme** — odeme_id, kayıt, tutar, yöntem, durum, tarih
- **Bilet Tipi** — tip_id, etkinlik, ad, fiyat, kontenjan, durum
- **Sertifika** — sertifika_id, katılımcı, etkinlik, oluşturma tarihi, durum
- **Rozet** — rozet_id, ad, ikon, açıklama, kriter
- **Anket** — anket_id, etkinlik, soru, tür
- **Anket Cevabı** — cevap_id, anket, katılımcı, cevap
- **Bildirim** — bildirim_id, başlık, mesaj, tür, okunma durumu
- **Kullanıcı** — kullanici_id, ad, soyad, kullanıcı adı, SHA256 parola, rol
- **Aktivite Log** — kullanıcı, işlem, tablo, kayıt_id, zaman

---

### Kullanıcı sistemde hangi işlemleri gerçekleştirebilir?

**Admin:**
- Kullanıcı ekleyebilir, düzenleyebilir, pasife alabilir
- Sistem ayarlarını güncelleyebilir, DB yedeği alabilir
- Aşağıdaki tüm organizatör işlemlerini yapabilir

**Organizatör:**
- Etkinlik ekleyebilir, düzenleyebilir, iptal edebilir, arayabilir
- Katılımcı ekleyebilir, düzenleyebilir, pasife alabilir
- Kayıt (bilet) oluşturabilir, iptal edebilir
- Bekleme listesini yönetebilir, yer açıldığında kayıta dönüştürebilir
- Oturum ve konuşmacı ekleyebilir, güncelleyebilir
- Ödeme kaydedebilir, iade işlemi yapabilir
- Bilet tipi tanımlayabilir ve düzenleyebilir
- Sertifika oluşturabilir (tekli veya toplu)
- Anket oluşturabilir ve sonuçlarını görüntüleyebilir
- Bildirimleri görüntüleyebilir, okundu işaretleyebilir
- İstatistik ve gelişmiş analizleri görüntüleyebilir
- Excel ve CSV raporu export edebilir
- Aktivite logunu görüntüleyebilir

---

## 🖥️ Teknolojiler

| Teknoloji | Kullanım Alanı |
|-----------|----------------|
| Python 3.9+ | Ana programlama dili |
| PyQt5 | GUI Framework |
| SQLite3 | Veritabanı yönetimi (`@contextmanager`) |
| QPainter | Tüm grafikler (Bar, Pie, Line) |
| hashlib (SHA256) | Şifre güvenliği |
| openpyxl / csv | Rapor export |
