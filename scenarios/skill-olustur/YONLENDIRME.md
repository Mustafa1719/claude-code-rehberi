# Skill Oluşturma Alıştırması

Bu klasör Ders 3-1 için hazırlanmıştır.

Aşağıdaki soruları cevaplayarak kendi ilk skill'ini oluşturacaksın.

---

## Adım 1: Tekrar Eden İşini Bul

Şu soruları kendine sor:

- Haftada en az 2-3 kez yaptığın ama sıkıcı bulduğun iş nedir?
- Her seferinde Claude'a aynı talimatları tekrar tekrar yazmak zorunda kaldığın bir iş var mı?
- "Keşke bir kez tanımlasam ve hep hatırlasa" dediğin bir şey var mı?

**Yaygın örnekler:**
- Toplantı notlarını belirli bir formata çevirmek
- E-postaları özetlemek
- Haftalık durum raporu yazmak
- Sosyal medya içeriği taslağı oluşturmak
- Müşteri görüşme notu düzenlemek
- Veri setini belirli bir formata dönüştürmek

---

## Adım 2: Skill'i Tanımla

Seçtiğin iş için şunları belirle:

**İsim:** Skill'in adı ne olacak? (kısa, tire ile, örn: `toplanti-notu`, `haftalik-rapor`)

**Tetikleyici:** Nasıl çağıracaksın? (örn: `/toplanti-notu`)

**Girdi:** Skill'e ne veriyorsun? (bir dosya, bir metin, bir liste?)

**Çıktı:** Skill ne üretiyor? (bir liste, bir rapor, bir email?)

**Format:** Çıktı nasıl görünmeli? (maddeler, tablo, paragraf?)

**Dil:** Türkçe mi, İngilizce mi?

---

## Adım 3: Skill'i Yaz

Bu soruların cevaplarını topladıktan sonra Claude'a şunu söyle:

```
Bu bilgilere göre benim için bir SKILL.md dosyası oluştur:
İsim: [skill adı]
Tetikleyici: /[komut]
Girdi: [ne veriyorsun]
Çıktı: [ne üretiyor]
Format: [nasıl görünmeli]
Dil: Türkçe
```

---

## Örnek: Toplantı Notu Skill'i

```markdown
# Toplantı Notu Özeti

**Tetikleyici:** /toplanti-notu
**Açıklama:** Toplantı notlarını yapılandırılmış özete dönüştür

## Giriş
Kullanıcıdan toplantı notlarını iste (dosya veya yapıştırılmış metin).

## Adımlar
1. Notu oku
2. Toplantı bilgilerini çıkar: tarih, katılımcılar, konu
3. Alınan kararları listele (madde işareti)
4. Görevleri listele: görev — sorumlu kişi — termin
5. Açık sorular varsa listele
6. Türkçe, madde işareti formatında sun

## Çıktı Formatı
## Toplantı Özeti
**Tarih:** [tarih]
**Katılımcılar:** [liste]

### Kararlar
- [karar 1]
- [karar 2]

### Görevler
- [ ] [görev] — [kişi] — [termin]

### Açık Sorular
- [soru]
```
