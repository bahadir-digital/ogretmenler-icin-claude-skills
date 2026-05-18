---
name: parent_meeting_summarizer
description: Veli toplantısı sırasında alınan dağınık notları yapılandırılmış toplantı özetine dönüştürür. Konu başlıklarına ayırır, alınan kararları, açılan tartışmaları, sonraki adımları ve sorumluları çıkarır. Öğretmen "veli toplantısı notlarını düzenle", "toplantı özeti", "veli toplantısı raporu", "tutanak hazırla" gibi ifadeler kullandığında devreye gir.
---

# Veli Toplantısı Özetleyici

Dağınık toplantı notlarını okunabilir, paylaşılabilir özete dönüştürür.

## Ne zaman tetiklenir

- "Veli toplantısı notlarımı düzenle"
- "Toplantı özeti hazırla"
- "Velilere paylaşacağım toplantı raporu"
- "Bu notlardan tutanak çıkar"

## Girdi olarak iste

1. **Toplantı notları** (yapıştırılmış metin, sesli not transkripti, dosya yüklemesi)
2. **Toplantı bilgisi:** Tarih, sınıf, katılan veli sayısı (yaklaşık)
3. **Format tercihi:** Veliyle paylaşılacak resmi rapor / idare için iç tutanak / öğretmenin kendi takip notu
4. **Çıkarılacak şeyler var mı?** Veli isimleri, kişisel detaylar gibi

## Çıktı yapısı

```
VELİ TOPLANTISI ÖZETİ

GENEL BİLGİLER
- Tarih: 
- Sınıf:
- Toplantıyı yürüten: 
- Katılım: X / Y veli
- Süre: 

GÜNDEM
1. [Konu başlığı]
2. [Konu başlığı]
3. ...

KONULAR VE TARTIŞMALAR

1. [Konu başlığı]
   Sunulan: [Öğretmen ne anlattı]
   Tartışma: [Veliler ne sordu, ne dedi]
   Sonuç: [Karar / öneri / aksiyon]

2. ...

ALINAN KARARLAR
- [Madde madde, net karar cümleleri]
- ...

YAPILACAKLAR (ACTION ITEMS)
| Yapılacak | Sorumlu | Tarih |
|-----------|---------|-------|
| ...       | ...     | ...   |

BİR SONRAKİ TOPLANTI
[Tarih ve gündem önerisi varsa]
```

## Kurallar

### Bilgi temizleme

- **Veli isimlerini özet metninde geçirmemek** (eğer "veliyle paylaşılacak rapor" istendiyse). Onun yerine "bir veli", "katılımcılardan biri".
- **Çocuk isimleri ne zaman yazılır?** Toplu toplantıda genelde yazılmaz. "Bir öğrencinin durumu" şeklinde anonim tut. Eğer öğretmenin kendi takip notuysa isim yazılabilir.
- **Yan konuşmaları çıkar.** "Veliler arasında çay sohbeti", "Geç gelen velinin selamlaşması" gibi unsurlar özetin parçası değil.

### Yapılandırma

- **Konuşma sırası önemli değil.** Toplantıda 3. konu açıldı, sonra 1. konuya dönüldü — özette konu bazında topla.
- **Tekrarlanan endişeleri konsolide et.** 5 veli aynı şikayeti dile getirdiyse, "Birden fazla veli şu konuyu dile getirdi" şeklinde tek noktada yaz.
- **Aksiyon maddesi olmayan tartışmaları kısa tut.** Sonuçsuz tartışma 5 satır olmasın.

### Karar yazımı

- **Net, ölçülebilir, sorumlusu belli.**
- Kötü: "Daha çok ödev yapılacak."
- İyi: "Her hafta cuma günü öğretmen, yapılmayan ödevleri WhatsApp grubunda toplu paylaşacak."

### Hassas konular

Toplantıda kişisel/zor bir konu açıldıysa (boşanma, hastalık, ekonomik zorluk):

- **Resmi rapora yazma.**
- **İç tutanakta** "Öğretmen rehberlik servisine bireysel görüşme önerdi" gibi nötr ifadeyle geçiştir.
- **Asla detay paylaşma.**

### Tartışmalı / hararetli konu

Eğer toplantıda tartışma çıktıysa:

- **Suçlayıcı dilden uzak yaz.**
- **Tarafların pozisyonlarını dengeli sun:** "Bazı veliler X dedi, diğerleri Y dedi."
- **Çözüm önerisi ya da bir sonraki adıma odaklan.**

### Format farkları

**Veliyle paylaşılacak resmi rapor:**
- Profesyonel ton
- İsim ve detaylar anonim
- "Saygılarımla, [Öğretmen]" şeklinde imzayla biter
- WhatsApp grubuna kopyala-yapıştır için kısa versiyon da öner

**İdare için iç tutanak:**
- Tüm detaylar (isim dahil) olabilir
- İmza yeri bırak
- Resmi tutanak formatına uygun

**Öğretmenin kişisel takip notu:**
- Kısa, madde madde olabilir
- Öğretmenin kendi yorum/gözlem notları eklenebilir
- "X velisi ile sonra bireysel konuşmalıyım" gibi kişisel hatırlatmalar yer alabilir

## Veliyle paylaşılacak kısa WhatsApp özeti

Resmi raporun yanında, gruba atılabilecek 5-7 satırlık özet de sun:

```
Değerli velilerimiz,

[Tarih]'te yaptığımız toplantıda görüşülen ana konular:

- [Madde 1]
- [Madde 2]
- [Madde 3]

Alınan kararlar:
- [Karar 1]
- [Karar 2]

Katılım için teşekkür ederim.
[Öğretmen]
```

## Örnek girdi

[Yapıştırılmış dağınık not bloğu]
"toplantı 15.30 başladı. ahmet'in annesi geç geldi. matematik konusu açıldı, çoğunluk müfredatın hızlı olduğunu söyledi. öğretmen kazanım tablosunu gösterdi. ödev miktarı tartışıldı, bazı veliler az dedi, bazıları çok. iki haftada bir küçük sınav yapılması kararlaştırıldı. ahmet'in babası okula bağış konusunu sordu, idareye yönlendirildi..."
