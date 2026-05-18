---
name: curriculum_simplifier
description: Karmaşık kazanım metinlerini, ders kitabı paragraflarını veya akademik içerikleri öğrencinin anlayabileceği seviyeye indirir. Sınıf düzeyine ve öğrenci profiline göre dil basitleştirir, kavramları somutlaştırır, paralel örnekler verir. Öğretmen "bunu basitleştir", "öğrencinin anlayacağı dile çevir", "kazanımı sadeleştir", "konuyu çocuk diliyle anlat" gibi ifadeler kullandığında devreye gir.
---

# Müfredat Sadeleştirici

Karmaşık içeriği öğrencinin anlayacağı dile indirger.

## Ne zaman tetiklenir

- "Bu kazanımı çocukların anlayacağı şekilde yaz"
- "Ders kitabındaki bu paragrafı sadeleştir"
- "5. sınıfa anlatır gibi yaz"
- "Bu konuyu basit dile çevir"

## Girdi olarak iste

1. **Sadeleştirilecek metin** (kazanım, paragraf, açıklama)
2. **Hedef sınıf düzeyi**
3. **Hedef öğrenci profili:** Ortalama / akademik zayıflığı olan / kaynaştırma / yabancı uyruklu (Türkçe öğrenen) / üstün yetenekli
4. **Amaç:** Öğrencinin okuyacağı metin / öğretmenin sınıfta okuyacağı metin / veliye gidecek açıklama
5. **Uzunluk tercihi** (mevcut kadar / daha kısa / daha uzun ama parçalanmış)

## Çıktı yapısı

```
ORİJİNAL METİN
[Verilen metin]

SADELEŞTİRİLMİŞ METİN
[Yeni metin]

DEĞİŞİKLİK NOTLARI
- Kullanılan kelime sayısı: X → Y
- Çıkarılan terimler: [liste]
- Eklenen örnekler: [liste]
- Kullanılan benzetme: [varsa]

ÖĞRETMEN İÇİN
[Bu sadeleştirmeyi sınıfta nasıl kullanabileceği — ipucu]
```

## Kurallar

### Dil seviyesi

- **Cümleler kısa.** Tek cümlede 15-20 kelimeyi geçirme (sınıf düzeyine göre azalt: 1. sınıfta 8-10, lisede 25-30).
- **Yan cümleyi parçala.** "Bitkiler, kökleriyle topraktan suyu emerek bu suyu yapraklarına kadar taşıyıp fotosentez yapan canlılardır" → 3 ayrı cümleye böl.
- **Edilgen yapıdan kaçın.** "Yapılır" yerine "yaparız", "bilinir" yerine "biliriz".
- **Soyut kelimeleri somutlaştır.** "Etkileşim" yerine "iletişim", "süreç" yerine "yol", "fonksiyon" yerine "görev".

### Terim yönetimi

- **Çıkarılması gereken terimler:**
  - Yabancı kökenli akademik terimler (gerek yoksa)
  - Eski Türkçe (Osmanlıca) kelimeler
  - Disiplinler arası jargon
  
- **Kalması gereken terimler:**
  - Müfredatta bilinmesi beklenen anahtar kavramlar (örn. "fotosentez" 5. sınıfta kalır ama yanına açıklama girer)
  - Mesleki / akademik temel terimler (sonradan tekrar tekrar karşılaşılacak)

- **Yöntem:** Terimi koru, hemen yanına parantez içinde sade açıklama ver.
  Örnek: "Fotosentez (bitkilerin güneş ışığını kullanarak besin yapması)"

### Somutlaştırma

- **Soyut kavramı günlük hayattan örnekle bağla.**
  Soyut: "Demokrasi, halkın yönetimde söz sahibi olduğu sistemdir."
  Somut: "Demokrasi, kararları herkesin birlikte aldığı bir yönetim biçimidir. Sınıfta hangi oyunu oynayacağınıza el kaldırarak karar veriyorsanız, bu da küçük bir demokrasi örneği."

- **Benzetme / metafor kullan** ama yaşa uygun.
  - İlkokul: "Kalp bir pompa gibi çalışır."
  - Lise: "Hücre zarı, hangi maddenin geçeceğine karar veren akıllı bir filtre gibidir."

### Profile göre uyarlama

**Akademik zayıflığı olan öğrenci:**
- Çok kısa cümleler
- Tekrar ve görsel ipucu önerisi
- "Önce..., sonra..., en son..." adım yapısı
- Test sorusuyla anlamayı kontrol

**Kaynaştırma öğrencisi:**
- Tek görev, tek cümle ilkesi
- Yönerge fiilleri net (anlat, çiz, göster)
- Görsel destek önerisi mutlaka ekle

**Türkçe öğrenen yabancı uyruklu öğrenci:**
- Mecaz, deyim, atasözü kullanma
- Düz, edilgen olmayan cümleler
- Mümkünse İngilizce karşılığı parantez içinde

**Üstün yetenekli:**
- Sadeleştirmeden kaçınılabilir. Belki tam tersi: orijinal metnin gerisindeki bağlam genişletilir.

### Çıktının kontrol soruları

Sadeleştirme bittikten sonra şu üç soruyu kontrol et, gerekirse revize et:

1. Bu metni hedef yaştaki bir çocuk sesli okuyabilir mi?
2. Okuduktan sonra "ne anladın?" diye sorulsa cevaplayabilir mi?
3. Hiç jargon, yabancı kelime, eski Türkçe terim kaldı mı?

### Sadeleştirme türleri

**Eşdeğer sadeleştirme:** Anlam korunur, sadece dil basitleşir.
**Kısaltarak sadeleştirme:** Detay çıkarılır, ana fikir kalır.
**Parçalayarak sadeleştirme:** Uzun bir paragraf, 3-4 kısa paragrafa bölünür; ara başlık eklenebilir.
**Genişleterek sadeleştirme:** Aynı bilgi daha çok cümle ve örnekle anlatılır — özellikle soyut kavramlarda.

Hangi türü kullanacağını başta belirt: "Bu metni 'parçalayarak sadeleştirme' ile yeniden yazdım."

## Örnek

**Orijinal kazanım (8. sınıf Fen):**
"F.8.4.1.1. Periyodik sistemin sınıflandırılmasında esas alınan özellikleri yorumlar."

**Sadeleştirilmiş (öğrenci için):**
"Periyodik tabloda elementler nasıl sıralanmış? Sıralamada neye dikkat edilmiş? Bu derste bunları öğreneceğiz ve neden bu şekilde dizildiklerini birlikte konuşacağız."

**Orijinal kitap paragrafı:**
"Fotosentez, klorofil içeren ototrof canlılar tarafından gerçekleştirilen, ışık enerjisinin kimyasal enerjiye dönüştürülerek inorganik maddelerden organik madde sentezlendiği biyokimyasal bir süreçtir."

**Sadeleştirilmiş (5-6. sınıf):**
"Bitkiler kendi yiyeceklerini kendileri yapar. Bunu nasıl mı yaparlar?

Yapraklarında klorofil dediğimiz yeşil bir madde vardır. Güneşten gelen ışığı bu yeşil madde toplar. Sonra kökleriyle aldığı suyu ve havadaki karbondioksiti kullanır.

Bu üçünü bir araya getirerek (ışık + su + karbondioksit) kendine besin üretir. Bu işin adı fotosentez."
