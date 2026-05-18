# Öğretmenler İçin Claude Skills

Öğretmenler için Claude Skill ve Project şablonları. Ders planından karne yorumuna, BEP'ten veli mektubuna — hafta sonlarını geri kazandıracak hazır kurulum.

## İçerik

### Project Instructions
- [`PROJECT_INSTRUCTIONS.md`](./PROJECT_INSTRUCTIONS.md) — Claude.ai Project'e yapıştırılacak talimat şablonu

### 10 Skill

| # | Skill | Klasör | Ne işe yarar |
|---|-------|--------|--------------|
| 1 | Ders Planı Oluşturucu | [`lesson_plan_creator`](./lesson_plan_creator) | MEB formatında ders planı |
| 2 | Sınav Soruları Üretici | [`exam_questions_producer`](./exam_questions_producer) | Çoktan seçmeli, boşluk doldurma, açık uçlu |
| 3 | Velilere Mektup Yazıcı | [`parent_letter_writer`](./parent_letter_writer) | Bilgilendirme, olumsuz durum, davet |
| 4 | BEP Hazırlayıcı | [`iep_preparer`](./iep_preparer) | Kaynaştırma öğrencisi için bireysel plan |
| 5 | Etkinlik & Oyun Tasarımcısı | [`classroom_activity_designer`](./classroom_activity_designer) | Konuya uygun sınıf içi etkinlik |
| 6 | Karne Yorumu Yazıcı | [`report_card_commenter`](./report_card_commenter) | Klişesiz, kişisel karne yorumu |
| 7 | Slayt İçerik Üreticisi | [`slide_content_creator`](./slide_content_creator) | Sunum yapısı + içerik |
| 8 | Ödev Değerlendirici | [`homework_evaluator`](./homework_evaluator) | Rubrik bazlı puanlama + geri bildirim |
| 9 | Veli Toplantısı Özetleyici | [`parent_meeting_summarizer`](./parent_meeting_summarizer) | Dağınık notu özete çevirir |
| 10 | Müfredat Sadeleştirici | [`curriculum_simplifier`](./curriculum_simplifier) | Karmaşık metni öğrenci diline indirger |

## Kurulum

1. Claude.ai → **Projects** → **Create project**
2. **Name:** Sınıfım (veya istediğin)
3. **Description:** Bu Project'in ne işe yaradığını kısaca yaz
4. **Instructions:** [`PROJECT_INSTRUCTIONS.md`](./PROJECT_INSTRUCTIONS.md) içeriğini kendine göre uyarla, yapıştır
5. Project oluştuktan sonra her bir `SKILL.md` dosyasını Skills bölümüne ekle

Detaylı kurulum kılavuzu: [bahadir.bearblog.dev](https://bahadir.bearblog.dev)

## Topluluk

- **WhatsApp:** [Claude.ai Türkiye](https://chat.whatsapp.com/I2763pKIpmS9xADAHLaGPE)
- **Instagram:** [@isicin.ai](https://www.instagram.com/isicin.ai/)
- **Blog:** [bahadir.bearblog.dev](https://bahadir.bearblog.dev)

## Başka mesleklere de gelecek

Bu repo öğretmenler içindir. Diğer meslek serileri (müşteri hizmetleri, finans, İK, satış, hukuk vb.) ayrı repolara yayımlanacak. Listeyi blogdan takip edebilirsin.

## Katkı

Pull request'e açık. İyileştirme, hata düzeltmesi, yeni skill önerisi — hepsi welcome.

## Lisans

MIT. Skill'leri istediğin yerde, istediğin gibi kullan. Atıf zorunlu değil ama görürsen sevinirim.
