---
name: lesson_plan_creator
description: MEB formatına uygun ders planı hazırlar. Konu, sınıf düzeyi, süre verildiğinde kazanım, yöntem, materyal, etkinlik akışı ve değerlendirme bölümlerini içeren tam ders planı çıkarır. Öğretmen "ders planı yaz", "bu konu için plan hazırla", "günlük plan", "yıllık plan" gibi ifadeler kullandığında devreye gir.
---

# Ders Planı Oluşturucu

MEB müfredatıyla uyumlu, sınıfta kullanılabilir ders planı hazırlar.

## Ne zaman tetiklenir

- "Şu konuya ders planı yaz"
- "5. sınıf İngilizce için Present Continuous planı"
- "40 dakikalık ders planı"
- "Günlük plan", "haftalık plan", "yıllık plan"

## Girdi olarak iste

Eğer kullanıcı bunları söylemediyse sor:

1. **Konu / kazanım kodu** (örn. "İ.5.3.1 — Selamlaşma ifadelerini ayırt eder")
2. **Sınıf düzeyi**
3. **Ders süresi** (40 dk standart, blok ders için 80 dk)
4. **Öğrenci sayısı ve seviye** (Project Instructions'ta yoksa)
5. **Özel istek varsa:** sınıf dışı etkinlik, dijital materyal, oyun bazlı vb.

## Çıktı yapısı

Aşağıdaki başlıklarla, sırayla yaz:

```
DERS BİLGİSİ
- Ders: 
- Sınıf: 
- Süre: 
- Tarih: [boş bırak, öğretmen doldursun]
- Ünite: 
- Konu: 
- Kazanımlar: [kod + metin halinde]

ÖĞRETİM YÖNTEM VE TEKNİKLERİ
[Anlatım, soru-cevap, beyin fırtınası, rol oynama, vb. — konuya uygun 2-4 tane]

KULLANILACAK MATERYALLER
[Ders kitabı sayfa numarası, tahta, projeksiyon, kartlar, video linki vb.]

DERS AKIŞI

1. Giriş (5-10 dk)
   - Dikkat çekme
   - Güdüleme
   - Gözden geçirme / ön bilgi yoklaması

2. Gelişme (20-25 dk)
   - Konunun işlenişi
   - Etkinlik / örnekler
   - Öğrenci katılımı

3. Sonuç (5-10 dk)
   - Özet
   - Değerlendirme
   - Bir sonraki derse hazırlık

DEĞERLENDİRME
[Şekillendirici / düzey belirleyici, hangi yöntemle: sözlü, yazılı, gözlem vb.]

ÖDEV / EV ÇALIŞMASI
[Varsa yaz, yoksa "ödev verilmemiştir" yaz]
```

## Kurallar

- **Kazanım kodlarını** mutlaka kullan (MEB formatı: ders kodu + sınıf + ünite + kazanım sırası).
- **Süre dağılımı** dengeli olsun; gelişme bölümü toplam sürenin yarısından az olamaz.
- **Etkinlikler** öğrenci profiline uygun olsun (Project Instructions'tan oku).
- **Materyal listesinde** öğretmenin önceden hazırlaması gerekenleri ayrıca işaretle.
- Plan içinde belirsizlik bırakma; "öğretmen burada uygun bir etkinlik yapar" gibi cümleler yazma — somut etkinliği ver.
- Birden fazla kazanım varsa, hangisinin baskın olduğunu belirt.

## Örnek girdi

"5. sınıf İngilizce, Present Continuous tense'e giriş, 40 dakika"

## Örnek çıktıdan kesit

```
KAZANIMLAR
İ.5.4.1 — Present Continuous Tense'i olumlu cümlelerde kullanır.
İ.5.4.2 — Görsellerdeki eylemleri Present Continuous ile ifade eder.

DERS AKIŞI

1. Giriş (8 dk)
   - Dikkat çekme: Öğretmen sınıfta yürür, kapıyı açar, oturur. 
     Her hareketi sonrasında "What am I doing?" diye sorar.
   - Güdüleme: "Şu anda" yapılan eylemleri İngilizce nasıl söyleriz?
     Türkçedeki "-yor" ekiyle bağlantı kur.
...
```
