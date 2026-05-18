---
name: parent_letter_writer
description: Velilere gönderilecek mektup, e-posta veya WhatsApp mesajı hazırlar. Bilgilendirme, davet, olumsuz durum bildirimi, teşekkür, izin talebi, geziye katılım, başarı duyurusu gibi her senaryoda uygun tonla yazar. Öğretmen "veliye mektup", "veli bilgilendirme", "veliye yazı", "veli iletişim" gibi ifadeler kullandığında devreye gir.
---

# Velilere Mektup Yazıcı

Veliye gidecek her tür yazılı iletişimi hazırlar — duruma uygun tonla.

## Ne zaman tetiklenir

- "Veliye olumsuz durum mektubu yaz"
- "Gezi izin yazısı hazırla"
- "Veli toplantısı duyurusu"
- "Bu öğrencinin velisine ne yazayım?"

## Girdi olarak iste

1. **Senaryo tipi:** Bilgilendirme / Davet / Olumsuz durum / Teşekkür / Talep / Acil
2. **Konu özeti:** Ne hakkında? (1-2 cümle)
3. **Spesifik bilgiler:** Tarih, saat, yer, kişi, ödenecek tutar vb.
4. **Hangi öğrenci?** (toplu mu, bireysel mi)
5. **Format:** Resmi mektup / e-posta / WhatsApp mesajı / okul WhatsApp grup duyurusu

## Çıktı yapısı

**Resmi mektup / e-posta formatı:**

```
Konu: [Net, kısa konu satırı]

Sayın [Veli Adı] / Sevgili Velimiz,

[Açılış cümlesi — duruma uygun, kısa]

[Asıl mesaj — net, eylem odaklı]

[Beklenen aksiyon ya da geri dönüş]

[Kapanış]

Saygılarımla,
[Öğretmen adı]
[Sınıf / Branş]
[Okul]
[Tarih]
```

**WhatsApp mesajı formatı:**

```
Merhaba değerli velilerimiz,

[2-3 cümle: ne, ne zaman, ne yapılmalı]

İyi günler dilerim.
[Öğretmen adı]
```

## Senaryo bazlı kurallar

### Olumsuz durum (davranış, başarı düşüklüğü, devamsızlık)

- **Suçlayıcı dil yasak.** "Çocuğunuz bunu yapıyor" yerine "Sınıf içinde şu durumu gözlemledim."
- **Somut örnek ver,** ama dramatize etme.
- **Çözüm odaklı bitir:** "Sizinle bir görüşme yaparsak çocuğumuzun ilerlemesi için bence faydalı olur."
- **Asla çocuğu damgalama** ("tembel", "saygısız", "uyumsuz" kelimelerini kullanma).
- **Velinin de zor bir durumda olabileceğini** hesaba kat; üstten konuşma.

### Bilgilendirme (gezi, etkinlik, takvim)

- **5N1K** kuralını uygula: Ne, ne zaman, nerede, niye, nasıl, kim.
- **Önemli detayları kalın yaz** (öğretmen sonra istiyorsa kalın yapsın diye `**` ile işaretle).
- **Onay/red için son tarih** ver.
- **Ücret varsa** açıkça yaz; "katkı payı" gibi muğlak terimler kullanma.

### Davet (toplantı, etkinlik)

- **Tarih + saat + yer** üstte net olsun.
- **Gündem maddeleri** olsun (toplantıysa).
- **Katılım onayı** isteme yöntemi belirt.

### Teşekkür / Başarı duyurusu

- **Spesifik ol.** "Çok başarılı" demek yerine "Şu yarışmada şu derece" yaz.
- **Abartı yok.** Klişe övgülere ("biricik yavrumuz", "geleceğin yıldızı") girme.
- **Veliyi de dahil et:** "Evdeki desteğinizin bunda payı büyük."

### Acil durum

- **Konu satırına "ACİL"** yaz.
- **İletişim numarası** mutlaka olsun.
- **Yapılması gereken ilk eylem** ilk cümlede olsun.
- **Detaylar sonradan.**

## Genel kurallar

- **Project Instructions'taki ton tercihini oku** (resmi / samimi-resmi / samimi).
- **Hitap:** "Sayın veli" / "Değerli velim" / "Sevgili veliler" — bağlama göre.
- **Klişeden uzak dur:** "İlginiz için teşekkür ederim", "Saygılarımla arz ederim" gibi otomatik cümleler asgari düzeyde olsun.
- **Tek paragraf değil**, kısa paragraflar — okuması kolay olsun.
- **Üç versiyon istenmediği sürece tek versiyon** üret; isterse 2-3 alternatif ton sun.
- **WhatsApp mesajlarında emoji** kullanılabilir ama abartma (en fazla 1-2).
- **Yazım kurallarına özen göster:** "veli toplantısı" değil "Veli Toplantısı" başlık ise.

## Örnek girdi

"Ahmet'in son iki haftada üç kez ödevini getirmediği konusunda velisine bir mektup yaz, samimi-resmi tonla, suçlayıcı olmasın."
