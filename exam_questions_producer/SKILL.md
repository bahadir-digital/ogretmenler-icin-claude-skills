---
name: exam_questions_producer
description: Belirtilen konu, sınıf düzeyi ve format için sınav soruları üretir. Çoktan seçmeli, boşluk doldurma, açık uçlu, eşleştirme, doğru-yanlış ve klasik soru tiplerini destekler. Her soru için cevap anahtarı ve zorluk seviyesi ekler. Öğretmen "sınav hazırla", "soru üret", "yazılı yoklama", "quiz", "test sorusu" gibi ifadeler kullandığında devreye gir.
---

# Sınav Soruları Üretici

Konu ve formata göre, cevap anahtarlı sınav soruları hazırlar.

## Ne zaman tetiklenir

- "10 tane çoktan seçmeli soru yaz"
- "Yazılı sınav hazırla"
- "Bu konudan quiz üret"
- "Ara sınav, dönem sonu, deneme sınavı"

## Girdi olarak iste

1. **Konu / ünite / kazanım**
2. **Soru sayısı**
3. **Soru tipi** (birden fazla olabilir): çoktan seçmeli, boşluk doldurma, eşleştirme, doğru-yanlış, açık uçlu, klasik
4. **Zorluk dağılımı** (örn. "%30 kolay, %50 orta, %20 zor")
5. **Sınav süresi** (puanlama dengesi için)

## Çıktı yapısı

```
SINAV BİLGİSİ
- Ders / Sınıf: 
- Konu: 
- Süre: 
- Toplam puan: 
- Soru sayısı:

═══════════════════════════════════
ÖĞRENCİ SINAV KAĞIDI
═══════════════════════════════════

A) ÇOKTAN SEÇMELİ SORULAR (her biri X puan)

1. [Soru metni]
   a) ...
   b) ...
   c) ...
   d) ...

2. ...

B) BOŞLUK DOLDURMA (her biri X puan)

...

═══════════════════════════════════
ÖĞRETMEN CEVAP ANAHTARI
═══════════════════════════════════

A) ÇOKTAN SEÇMELİ
1. c) — [neden doğru, kısa açıklama]
   Zorluk: Orta | Kazanım: İ.5.4.1

2. ...
```

## Kurallar

- **Cevap anahtarı ayrı bölümde** ver, asla soruyla aynı sayfada yazma.
- **Her soruya zorluk etiketi** koy: Kolay / Orta / Zor.
- **Her soruya kazanım kodu** ekle (Project Instructions'tan oku).
- **Çoktan seçmelide** çeldiriciler mantıklı olsun — rastgele yanlışlar yazma, öğrencinin yapabileceği tipik hataları yansıtsın.
- **Açık uçlu sorularda** beklenen cevap için anahtar kelimeleri/kavramları cevap anahtarında ver.
- **Puanlama** soru zorluğuyla orantılı: kolay 2-3 puan, orta 4-5 puan, zor 6-8 puan.
- **Toplam 100 puan** olacak şekilde dengele; çıkmıyorsa bonus soru ekle.
- **Yaş grubuna uygun dil** kullan; 5. sınıfa 11. sınıf dili yazma.
- **Görsel gerektiren soruları** "[Burada bir grafik/şekil olacak: tarif]" şeklinde işaretle, öğretmen ekleyecek.

## Soru tipi özel kuralları

**Çoktan seçmeli:** 4 seçenek standart. "Hepsi" ve "Hiçbiri" seçenekleri ölçme-değerlendirmede tercih edilmez, gerekmedikçe kullanma.

**Boşluk doldurma:** Bir cümlede en fazla 2 boşluk. Cevap tek kelime veya kısa ifade olmalı.

**Eşleştirme:** Sol sütun 5-7 madde, sağ sütun her zaman 1-2 fazla (çeldirici) olsun.

**Doğru-yanlış:** Cümleler net olsun, "bazen", "genellikle" gibi tartışmaya açık kelimeler kullanma.

**Açık uçlu:** Cevap için yer ayır (3-5 satır). Cevap anahtarında puan kırma kriterleri ver.

## Örnek girdi

"5. sınıf İngilizce, Present Continuous konusu, 10 çoktan seçmeli + 5 boşluk doldurma, 40 dakikalık sınav"
