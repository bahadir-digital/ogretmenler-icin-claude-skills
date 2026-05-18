---
name: slide_content_creator
description: Ders konusu için sunum slaytlarının içeriğini ve akışını hazırlar. Her slayt için başlık, ana içerik, görsel önerisi ve öğretmen notu verir. PowerPoint, Keynote, Canva, Google Slides'a doğrudan taşınabilecek formatta. Öğretmen "sunum hazırla", "slayt yap", "PowerPoint için içerik", "Canva için içerik", "ders sunumu" gibi ifadeler kullandığında devreye gir.
---

# Slayt İçerik Üreticisi

Sunumun yapısını, içeriğini ve görsel rehberini hazırlar.

## Ne zaman tetiklenir

- "Bu konuya sunum hazırla"
- "10 slaytlık ders sunumu"
- "PowerPoint için içerik üret"
- "Canva'da yapacağım, içeriği ver"

## Girdi olarak iste

1. **Konu**
2. **Sınıf düzeyi**
3. **Slayt sayısı** (varsayılan: 8-12)
4. **Sunum süresi** (ders saati / 20 dk / 5 dk)
5. **Hedef:** Ders anlatımı / tekrar / değerlendirme / ödev sunumu / veli sunumu
6. **Platform** (varsa): PowerPoint, Canva, Google Slides — fark eder, görsel önerileri buna göre olabilir

## Çıktı yapısı

Her slayt için ayrı blok:

```
SLAYT 1 — [Başlık tipi]
──────────────────────────

Başlık: [Net, kısa başlık]

İçerik:
[Tam metin — slayt üzerine yazılacak ya da öğretmenin söyleyeceği]

Görsel önerisi:
[Ne tür görsel? Foto / illüstrasyon / şema / grafik — kısa tarif]

Öğretmen notu:
[Sunum sırasında ne söylenecek, neye dikkat — slaytta yazmayacak ama önemli]

Süre tahmini: X dk
```

## Slayt yapı önerisi

Standart 10 slayt için akış:

| # | Tip | İçerik |
|---|-----|--------|
| 1 | Kapak | Başlık, sınıf, tarih |
| 2 | Isınma / Soru | Dikkat çekici giriş, "Sizce neden?" |
| 3 | Kazanımlar | Bu derste neyi öğreneceğiz (öğrenci diliyle) |
| 4-7 | Ana konu | Tek slayt = tek alt başlık |
| 8 | Uygulama / örnek | Soru, problem, vaka |
| 9 | Özet | 3-4 madde |
| 10 | Kapanış | Sonraki ders / ev ödevi |

## Kurallar

### Slayt başına içerik miktarı

- **Her slaytta en fazla 6 satır metin.** Yoğun paragraflar değil, kısa madde veya cümle.
- **Bir slayt = bir ana fikir.** Yarısı şu konu yarısı bu konu olmasın.
- **Başlık 7 kelimeyi geçmesin.**

### Görsel önerisi

- Spesifik öneri yap. "Bir resim" deme.
- Örnek: "Sınıfta bir öğrencinin pencereden dışarı baktığı yandan çekim fotoğraf."
- **Telif uyarısı** ver: "Pixabay, Unsplash veya benzeri telifsiz kaynak öneririm."
- **AI görsel** için prompt önerisi de ekleyebilirsin: "Midjourney/DALL-E için: '...'"

### Öğretmen notu (presenter notes)

- Slaytta görünmeyecek ama öğretmenin söyleyeceği şey.
- Öğretmenin **kelime kelime okuyacağı bir senaryo değil**, kısa hatırlatıcı.
- Etkileşim için soru önerileri: "Burada öğrencilere şunu sor: ..."

### Sunum türüne göre uyarlama

**Anaokulu / 1-2. sınıf:**
- Slaytlar çoğunlukla görsel olsun, az metin
- Renkli, eğlenceli görseller
- Tek slaytta tek fikir

**3-8. sınıf:**
- Görsel + kısa metin dengeli
- Animasyon önerisi olabilir (Canva için)
- İnteraktif elemanlar (soru-cevap slaytı)

**Lise:**
- Daha metin yoğun olabilir
- Grafikler, tablolar, kaynak referansı
- Akademik tonla

### Platform farkları

- **PowerPoint:** Smart Art, geçiş efektleri, animasyon önerebilirsin
- **Canva:** Şablon ismi önerebilirsin, hareketli sticker'lar mevcut
- **Google Slides:** İşbirliği özelliği vurgulanabilir, embed seçenekleri

## Çıktının sonuna ekle

```
ÖZET
- Toplam slayt: X
- Tahmini sunum süresi: X dk
- Hazırlanması gereken görsel sayısı: X
- Öğretmenin önceden hazırlaması gerekenler: ...
```

## Örnek girdi

"5. sınıf İngilizce, Present Continuous konusuna giriş, 10 slayt, 40 dakikalık ders, Canva'da yapacağım."

## Önemli not

Bu Skill **görsel üretmez**, sadece içerik ve yapı verir. Görselleri öğretmen kendisi Canva, PowerPoint ya da telifsiz kaynaklardan ekler. Görsel önerisi tarif şeklindedir, somut dosya değil.
