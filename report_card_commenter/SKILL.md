---
name: report_card_commenter
description: Karne arkasına yazılacak öğrenci yorumlarını hazırlar. Öğrencinin akademik durumu, davranışları ve sosyal gelişimi hakkında verilen kısa notlardan yola çıkarak kişisel, yapıcı, klişeden uzak yorumlar üretir. Öğretmen "karne yorumu yaz", "öğrenci yorumu", "rapor yorumu", "veliye karnede ne yazayım" gibi ifadeler kullandığında devreye gir.
---

# Karne Yorumu Yazıcı

Öğrenci için kişisel, klişeden uzak karne yorumu hazırlar.

## Ne zaman tetiklenir

- "Karne yorumu yaz"
- "Ahmet için karne arkasına yorum"
- "Bu öğrenciye ne yazayım?"
- "Sınıfımdaki 25 öğrenci için karne yorumu"

## Girdi olarak iste

1. **Öğrenci adı** (yoksa "öğrenci" olarak yaz)
2. **Sınıf düzeyi**
3. **Akademik durum:** Genel başarı seviyesi + güçlü/zayıf dersler
4. **Davranış / sosyal:** Sınıf içi tutumu, arkadaşlık ilişkileri
5. **Özel notlar:** Bu dönem öne çıkan bir gelişme, bir sorun, bir başarı
6. **Yorum tonu:** Olumlu / dengeli / yapıcı eleştirel

Toplu istek varsa tablo halinde iste:

```
| Öğrenci | Akademik | Davranış | Not |
| ------- | -------- | -------- | --- |
| Ahmet   | Orta+    | Aktif    | Matematikte ilerleme var |
| ...     | ...      | ...      | ... |
```

## Çıktı yapısı

Her öğrenci için 3-5 cümlelik bir paragraf. Yapı:

1. **Genel akademik durum** (somut)
2. **Güçlü taraf** (spesifik)
3. **Gelişim alanı** (yapıcı dille)
4. **Davranış / sosyal değerlendirme**
5. **Dönem hedefi / öneri** (geleceğe dönük)

## Kurallar

### Klişelerden kaçın

**Kullanma:**
- "Çok başarılı bir öğrenci"
- "Pırıl pırıl bir çocuk"
- "Her zaman olduğu gibi bu dönem de..."
- "Geleceğin parlak yıldızı"
- "Sınıfımızın gözbebeği"
- "Tertemiz bir kalbe sahip"
- "Daha çok çalışırsa daha iyi olacak"

**Kullan:**
- Spesifik dersler ("Türkçe okuma anlamada", "Matematikte problem çözmede")
- Spesifik davranışlar ("Grup çalışmalarında sorumluluk alıyor", "Söz alarak konuşma kuralına uymakta zorlanıyor")
- Spesifik gelişim noktaları ("Sunum yapmaktan çekinmesi azaldı", "Kalemini doğru tutmaya başladı")

### Olumsuz durumda

- **Asla damgalama yapma.** "Tembel", "saygısız", "sorunlu", "uyumsuz" kelimelerini KULLANMA.
- **Davranışı tanımla, çocuğu değil.** "Ödevini düzenli getirmedi" tamam, "ödev yapmayan biri" yanlış.
- **Çözüm odaklı kapanış.** "Önümüzdeki dönemde X konusuna odaklanırsak gelişme bekliyorum."
- **Velinin de okuyacağını unutma.** Aile içi sorunlara dair ima yapma.

### Olumlu durumda

- **Abartma.** "Olağanüstü" yerine "bu dönem belirgin ilerleme gösterdi" daha inandırıcı.
- **Sadece övmekle yetinme,** mutlaka bir gelişim alanı ekle. Aksi halde yorum sahte hissettirir.

### Tonal kurallar

- **3-5 cümle.** Daha uzun olmasın — karne arkası küçük yer.
- **Eğitsel jargon yok.** Veli okuyacak; "kazanım edinimi", "biliş üstü yetkinlik" gibi sözler yazma.
- **"Sizin çocuğunuz"** demek yerine **isimle ya da "öğrencimiz"** de.
- **Türkçe kurallarına özen** — virgüller, "de/da" ayrımı, büyük harf.

## Tekrardan kaçınma

Birden fazla öğrenci için yorum üretiyorsan, **aynı cümle yapılarını tekrar etme.** Her yorum farklı başlasın, farklı bitsin. 25 öğrenci için 25 farklı yapı kur.

## Örnek girdiler ve çıktılar

**Girdi:** "Elif, 5. sınıf, Türkçe çok iyi, matematikte zorlanıyor, sessiz ve içine kapanık, sunum yapmakta çekinir."

**Çıktı:**
"Elif, Türkçe dersinde okuma anlama ve kelime hazinesi yönünden sınıf ortalamasının üzerinde performans gösterdi. Matematikte özellikle problem çözme konusunda zorlandığı gözlendi; bu alanda evde ek çalışma faydalı olacaktır. Grup çalışmalarında çekingenliği zaman zaman katılımını sınırlasa da yazılı çalışmalarında düşüncelerini açık biçimde ifade ediyor. Önümüzdeki dönemde sözlü katılımı arttıracak küçük adımlar planlıyoruz."

**Girdi:** "Burak, 3. sınıf, hareketli, arkadaşlarıyla iyi geçinir ama derste söz almadan konuşur, ödevlerini düzenli getirmez."

**Çıktı:**
"Burak, sınıf arkadaşlarıyla olumlu ilişkiler kuran, paylaşımcı bir öğrencimizdir. Derste fikirlerini paylaşma konusunda istekli; ancak söz alma kuralına uyma konusunda destek almaya devam edecek. Ödev takibinde düzenli bir gelişme görmek için evde günlük bir rutin oluşturulması önemli olacaktır. Burak'ın enerjisini akademik çalışmaya yönlendirmek için bu dönem sınıf içi sorumluluklarını arttırmayı düşünüyoruz."

## Toplu üretim formatı

Çok sayıda öğrenci için istek geldiğinde, çıktıyı **isimle başlık olarak** ayır:

```
ELİF
[3-5 cümle]

BURAK
[3-5 cümle]

...
```
