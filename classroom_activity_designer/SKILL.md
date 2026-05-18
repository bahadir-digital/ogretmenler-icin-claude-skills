---
name: classroom_activity_designer
description: Ders konusuna ve süreye uygun sınıf içi etkinlik, oyun veya grup çalışması tasarlar. Malzeme listesi, adım adım uygulama yönergesi ve değerlendirme kriteri içerir. Öğretmen "etkinlik öner", "oyun tasarla", "grup çalışması", "drama", "isınma aktivitesi", "ders başında ne yapsam" gibi ifadeler kullandığında devreye gir.
---

# Etkinlik ve Oyun Tasarımcısı

Konuya, süreye ve sınıfa uygun, uygulanabilir etkinlikler hazırlar.

## Ne zaman tetiklenir

- "Bu konuya bir etkinlik öner"
- "5 dakikalık ısınma aktivitesi"
- "Grup çalışması için oyun"
- "Sınıfta canlandırma yapabileceğim bir şey"

## Girdi olarak iste

1. **Konu / kazanım**
2. **Etkinlik amacı:** Konuyu öğretmek / pekiştirmek / değerlendirmek / ısındırmak / motivasyon vermek
3. **Süre** (5 dk / 10 dk / 20 dk / tam ders)
4. **Sınıf düzeyi ve öğrenci sayısı**
5. **Kısıt varsa:** sıraları hareket ettirmeden, sessiz olmalı, sınıf dışında, vb.
6. **Malzeme imkanı:** sadece tahta, projeksiyon var mı, kağıt-kalem, fotokopi vb.

## Çıktı yapısı

```
ETKİNLİK ADI
[Akılda kalıcı bir isim ver]

KAPSAMI
- Konu / kazanım:
- Amaç: [Öğretme / pekiştirme / değerlendirme / ısınma]
- Süre: 
- Sınıf düzeyi:
- Öğrenci sayısı: [bireysel / 2-3 kişilik grup / 5-7 kişilik grup / tüm sınıf]

MALZEME LİSTESİ
- [Madde madde, miktarıyla birlikte]
- [Önceden hazırlanması gerekenler ⚠ ile işaretle]

UYGULAMA ADIMLARI

1. Hazırlık (X dk)
   - ...

2. Etkinlik (X dk)
   - Adım 1: ...
   - Adım 2: ...
   - Adım 3: ...

3. Kapanış (X dk)
   - Değerlendirme
   - Sınıfa geri dönüş

ÖĞRENCİ KAZANIMI
[Etkinlik sonunda öğrenci neyi yapabilir/anlayabilir hâle gelir]

DEĞERLENDİRME
[Nasıl ölçüleceği — gözlem, çıktı, sözlü vb.]

UYARLAMA NOTLARI
- Kalabalık sınıfta: ...
- Az zamanda: ...
- Kaynaştırma öğrencisi için: ...

OLASI SORUNLAR VE ÇÖZÜMLERİ
- [Sınıfta çıkabilecek aksaklık] → [Çözüm]
```

## Kurallar

- **Yaş grubuna uygun olsun.** Anaokuluna soyut kavram, lise sonuncuya boyama yaptırma.
- **Gerçekçi malzeme.** Türkiye'deki ortalama bir devlet okulunda olmayan şeyleri (3D yazıcı, robotik kit vb.) gerektirme. Project Instructions'taki okul tipini oku.
- **Adım adım, anlaşılır.** Öğretmen okuduğu anda uygulayabilmeli.
- **Süre yönetimi gerçekçi.** "5 dakikada 4 grup sunum yapsın" gibi imkansız tahminler verme.
- **Sınıf yönetimi düşün.** Öğrenciler ayağa kalkacaksa, gürültü olacaksa belirt.
- **Risk uyarısı:** Bedeni bir aktivite varsa "çarpışma riskine dikkat", makas/kalem kullanılıyorsa "güvenlik gözetimi" notu ekle.
- **Sadece eğlence değil, kazanım odaklı.** Her etkinliğin sonunda öğrenci ne öğrenmiş olacak — net.
- **Kaynaştırma öğrencisi için uyarlama** mutlaka olsun (uyarlama notları bölümü).

## Etkinlik tipi kategorileri

İhtiyaca göre bu tiplerden birini öner:

- **Isınma:** 3-5 dk, dikkat toplama, derse giriş köprüsü
- **Drama / canlandırma:** Rol dağılımı, yönlendirme, kısa süreli
- **Yarışma:** Bireysel veya takım, puanlama mekanizması belli
- **Bulmaca / problem çözme:** Tek başına ya da grup
- **İstasyon çalışması:** Sınıf 3-4 alana bölünür, gruplar dönüşümlü
- **Tartışma / münazara:** Konu verilir, savunma rolleri dağıtılır
- **Sanat / üretim:** Çizim, kolaj, model
- **Dijital etkinlik:** Kahoot, Wordwall, Mentimeter — link vermeden yapı öner
- **Sınıf dışı:** Bahçe, koridor, başka mekan

## Önemli

**"En bilinen" etkinlikleri tekrar tekrar önerme.** Tabu, mim oyunu, kelime zinciri gibi standartları çocuk her ders görüyor. Konuya özgü, yeni, ilginç bir şey tasarla.

## Örnek girdi

"5. sınıf İngilizce, Present Continuous konusunu pekiştirme, 15 dakika, sınıfta 24 öğrenci, fotokopi imkanı var, sıralarda kalsınlar."
