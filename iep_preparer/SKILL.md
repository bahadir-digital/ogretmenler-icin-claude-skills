---
name: iep_preparer
description: Kaynaştırma veya özel gereksinimli öğrenciler için Bireyselleştirilmiş Eğitim Planı (BEP) taslağı hazırlar. RAM raporuna uygun, MEB formatında, ölçülebilir kazanımlarla. Öğretmen "BEP yaz", "kaynaştırma planı", "bireysel eğitim", "özel öğrenci için plan", "RAM raporu için plan" gibi ifadeler kullandığında devreye gir.
---

# Bireysel Eğitim Planı (BEP) Hazırlayıcı

Kaynaştırma öğrencileri için ölçülebilir, gerçekçi BEP taslağı hazırlar.

## Ne zaman tetiklenir

- "Kaynaştırma öğrencim için BEP hazırla"
- "Bu öğrenciye bireysel eğitim planı"
- "RAM raporu sonrası plan"
- "Özel öğrenme güçlüğü olan öğrenci için ders planı"

## Girdi olarak iste

1. **Öğrencinin tanı/durumu** (RAM raporundan: hafif zihinsel yetersizlik, özel öğrenme güçlüğü, dikkat eksikliği, otizm spektrum, işitme/görme yetersizliği vb.)
2. **Sınıf seviyesi**
3. **Ders / alan** (BEP genelde ders bazlı yazılır)
4. **Öğrencinin mevcut performansı** (neyi yapabiliyor, neyi yapamıyor — somut)
5. **Plan dönemi** (yıllık / dönemlik / ünite bazlı)

## Çıktı yapısı

```
BİREYSELLEŞTİRİLMİŞ EĞİTİM PLANI (BEP)

ÖĞRENCİ BİLGİLERİ
- Ad-Soyad: 
- Sınıf: 
- Tanı / RAM Yönlendirmesi: 
- Plan dönemi: 
- BEP Sorumlusu: [Öğretmen adı]
- Hazırlanma tarihi: 

MEVCUT PERFORMANS DÜZEYİ (MPD)
[Öğrencinin şu an yapabildikleri ve yapamadıkları — somut, ölçülebilir]

UZUN DÖNEMLİ AMAÇ (Yıllık)
[Tek cümle, geniş kapsamlı hedef]

KISA DÖNEMLİ AMAÇLAR (Aylık/Dönemlik)
1. [Ölçülebilir, gözlenebilir, somut]
2. ...
3. ...

KAZANIMLAR (Sınıf kazanımından uyarlanmış)
- Orijinal kazanım: [MEB kodu + metin]
- Uyarlanmış kazanım: [öğrenci seviyesine indirgenmiş hâli]

ÖĞRETİM YÖNTEMLERİ VE UYARLAMALAR
- Sınıf içi yerleşim: 
- Materyal uyarlaması: 
- Süre uyarlaması: 
- Anlatım yöntemi: 
- Görsel/işitsel destek:

DEĞERLENDİRME UYARLAMASI
- Sınav formatı: 
- Sınav süresi: 
- Soru sayısı / tipi:
- Puanlama:

EV ÖDEVLERİ
[Öğrencinin yapabileceği seviyede, miktarda]

İLERLEME TAKİP YÖNTEMİ
[Haftalık gözlem, aylık değerlendirme, vb.]

İŞBİRLİĞİ
- Veli görüşmesi sıklığı: 
- Rehberlik servisi ile iletişim: 
- BEP geliştirme birimine geri bildirim:
```

## Kurallar

- **Kazanımlar ölçülebilir olsun.** "Toplama yapar" değil, "İki basamaklı doğal sayılarla 5/10 doğrulukla toplama işlemi yapar."
- **SMART hedef** kuralı: Specific (Belirli), Measurable (Ölçülebilir), Achievable (Ulaşılabilir), Relevant (İlgili), Time-bound (Süreli).
- **Sınıf kazanımından sapmayı belirt.** Hangi kazanımı tamamen alıyoruz, hangisini uyarlıyoruz, hangisini çıkarıyoruz — net olsun.
- **Tanıya uygun strateji öner.**
  - **Hafif zihinsel yetersizlik:** Tekrar, somutlaştırma, görsel destek, küçük adımlar.
  - **Özel öğrenme güçlüğü (disleksi/diskalkuli):** Yazılı yerine sözlü, ek süre, font/renk uyarlaması.
  - **Dikkat eksikliği:** Kısa görevler, ara molalar, ön sıra, görsel ipuçları.
  - **Otizm spektrum:** Rutin, ön bildirim, görsel program, duyusal uyaran kontrolü.
  - **İşitme yetersizliği:** Yüze dönük konuşma, yazılı destek, görsel materyal.
  - **Görme yetersizliği:** Büyük punto, dokunsal materyal, sözlü tarif.
- **Veliye gösterilecek dilde yaz.** Tanıyı damgalayıcı dille anlatma; öğrencinin güçlü yanlarını da belirt.
- **Hukuki çerçeve.** BEP, MEB Özel Eğitim Hizmetleri Yönetmeliği gereği zorunlu — bunu öğretmene hatırlatma şart değil ama plan formatı yasaya uygun olmalı.
- **Birden fazla ders varsa**, her ders için ayrı kısa dönemli amaç yaz.

## Önemli not

BEP, BEP Geliştirme Birimi tarafından onaylanır. Bu Skill'in ürettiği çıktı bir **taslak**tır. Öğretmen, rehber öğretmen, veli ve idare ile birlikte değerlendirilip kesinleşir. Çıktının sonuna şu notu ekle:

> *Bu taslak, BEP Geliştirme Birimi'nde değerlendirilmek üzere hazırlanmıştır. Veli, rehberlik servisi ve idare görüşü alındıktan sonra kesinleşir.*

## Örnek girdi

"4. sınıfta hafif düzey otizm tanılı kaynaştırma öğrencim var. Matematik dersinde 100 içinde toplama-çıkarma yapabiliyor ama çarpma henüz başlamadı. Dikkat süresi 10 dakika civarı. Bir dönemlik BEP hazırla."
