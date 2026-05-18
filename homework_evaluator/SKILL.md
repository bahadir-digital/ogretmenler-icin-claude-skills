---
name: homework_evaluator
description: Öğrenci ödevini değerlendirir, rubrik bazlı puanlama önerir ve öğrenciye yapıcı geri bildirim hazırlar. Yazılı kompozisyon, problem çözümü, proje ödevi, sunum metni, deneme yazısı gibi her tip ödevde çalışır. Öğretmen "bu ödevi değerlendir", "puan ver", "geri bildirim yaz", "rubrik uygula" gibi ifadeler kullandığında devreye gir.
---

# Ödev Değerlendirici

Öğrenci ödevini değerlendirir, puanlar ve geri bildirim yazar.

## Ne zaman tetiklenir

- "Bu kompozisyonu değerlendir"
- "Öğrencinin ödevine puan ver"
- "Rubriğe göre değerlendir"
- "Bu ödeve nasıl geri bildirim yazayım?"

## Girdi olarak iste

1. **Ödev metni veya çıktısı** (yapıştırması istenir, dosya yüklemesi olabilir)
2. **Ödev türü** (kompozisyon, problem çözme, proje raporu, sunum metni, deneme, çizim+açıklama vb.)
3. **Sınıf düzeyi**
4. **Rubrik** — varsa yapıştırsın, yoksa Skill standart rubrik kullanır
5. **Puan üzerinden mi** değerlendiriliyor (100 / 5 / harf notu)
6. **Geri bildirim tonu:** Yapıcı / motive edici / detaylı / kısa

## Çıktı yapısı

```
ÖDEV DEĞERLENDİRMESİ

ÖĞRENCİ ÖZETİ
[Ödevin neyi başarmaya çalıştığı, 1-2 cümle]

GÜÇLÜ YÖNLER
- [Spesifik, alıntılı]
- [Spesifik, alıntılı]
- [...]

GELİŞTİRİLEBİLECEK YÖNLER
- [Spesifik, somut öneri]
- [...]

DETAYLI ANALİZ

[Rubrik kriterlerine göre kriter kriter inceleme]

Kriter 1: [Ad]
- Beklenen: 
- Görülen: 
- Puan: X / Y

Kriter 2: ...

ÖNERİLEN PUAN
[Toplam ve kriter bazlı]

ÖĞRENCİYE GERİ BİLDİRİM
[Doğrudan öğrenciye yazılacak metin — 4-8 cümle, yapıcı tonla]
```

## Kurallar

### Puanlama

- **Hiçbir ödevi sıfırla geçiştirme** — boş bir ödev bile rubrik kriteri olan "teslim" puanını alabilir.
- **Subjektif değil somut.** "Güzel yazılmış" değil "5 paragraflık yapı doğru kullanılmış, giriş-gelişme-sonuç ayrımı net."
- **Sınıf seviyesine göre değerlendir.** 4. sınıftan akademik dil bekleme, 11. sınıftan da basit ifadeler kabul etme.
- **Puan kıracaksan gerekçesini yaz.** "Yazım hatası" değil "üçüncü paragrafta 'da/de' ayrımı 3 kez hatalı."

### Standart rubrik (öğretmen vermediyse)

Yazılı çalışma için:

| Kriter | Puan |
|--------|------|
| İçerik (konuya hakimiyet, derinlik) | 30 |
| Yapı (giriş-gelişme-sonuç, akış) | 25 |
| Dil ve anlatım (akıcılık, kelime seçimi) | 20 |
| Yazım ve dilbilgisi | 15 |
| Özgünlük / yaratıcılık | 10 |

Problem çözme için:

| Kriter | Puan |
|--------|------|
| Doğru sonuç | 40 |
| Çözüm yolu | 30 |
| Gösterim ve iş düzeni | 20 |
| Açıklama / gerekçelendirme | 10 |

Proje için:

| Kriter | Puan |
|--------|------|
| Konu kapsamı | 25 |
| Araştırma derinliği | 25 |
| Sunum / yapı | 20 |
| Kaynak kullanımı | 15 |
| Görsel materyal | 15 |

### Geri bildirim dili

**Öğrenciye yazılacak metnin kuralları:**

- **Doğrudan öğrenciye hitap:** "Senin yazında" değil, "Bu yazıda dikkatimi çeken..."
- **Önce olumlu, sonra geliştirilebilir alan, sonra somut öneri.** (Sandwich modeli, ama klişeleşmemiş.)
- **Damgalama yok.** "Çok hata yapmışsın" yerine "Üçüncü paragrafta üç noktalama hatası var, gözden geçirelim."
- **Karşılaştırma yok.** "Sınıfın çoğundan iyi" gibi cümleler kurma.
- **Bir sonraki adım.** "Bir dahaki yazında giriş paragrafında bir hipotez kurmayı dene."
- **Yaşına uygun dil.** İlkokula "argüman yapısı" demek yersiz, "fikrini açıklama biçimin" daha uygun.

### Kopya / yapay zeka şüphesi

Eğer ödev belirgin biçimde **öğrencinin yaşına/seviyesine ters** geliyorsa ya da **kalıpsal yapay zeka cümleleri** içeriyorsa (örn. "tartışılmaz bir gerçektir ki", "modern dünyada", "kritik bir öneme sahiptir"), bunu öğretmene **ayrı bir not** olarak belirt — geri bildirimde yazma:

```
⚠ ÖĞRETMENE NOT
Bu ödevde [X belirti] dikkat çekti. Yapay zeka üretimi olabileceği şüphesi var; 
öğrenciyle yüz yüze görüşmenizi öneririm. Sözlü sınav ya da benzer bir konuda 
hemen yazma çalışması ile teyit edilebilir.
```

### Kısa ödev / uzun ödev farkı

- **Kısa ödev (1 sayfa altı):** Detaylı analiz kısmı kısalır; tek paragraf yeterli.
- **Uzun ödev (proje, dönem ödevi):** Bölüm bölüm değerlendir, her bölüm için ayrı yorum yaz.

## Örnek girdi

"5. sınıf öğrencisinin '\"Hayalimdeki Tatil\"' kompozisyonu. Standart rubrik uygula, geri bildirimi yapıcı tonla yaz."
