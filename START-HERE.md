# Claude Code Rehberi

Türkçe, teknik bilgi gerektirmeyen, yaparak öğreten Claude Code kursu.

## Nasıl Başlanır?

```
START-HERE.md dosyasını oku ve kursa başla
```

Belirli bir derse atlamak için:

```
START-HERE.md dosyasını oku ve ders 2-2'den başla
```

## Gezinme Komutları

- **"başla"** → En baştan başla
- **"ders 1-2"** → Belirli bir derse atla
- **"devam"** veya **"sonraki ders"** → Bir sonraki derse geç
- **"kaldığım yerden devam et"** → İlerleme dosyasını oku, kaldığın yerden başla
- **"modül 3"** → O modülün ilk dersine git

---

## Kurs Haritası — 14 Ders, 5 Modül

### Modül 0: Neden? (~20 dk)
| Ders | Konu | Dosya |
|------|------|-------|
| 0-0 | Kurs nasıl çalışır? | `MODUL-0/00-hos-geldin.md` |
| 0-1 | ChatGPT'den farkı nedir? | `MODUL-0/01-neden-claude-code.md` |
| 0-2 | Claude Code nasıl "düşünür"? | `MODUL-0/02-buyuk-resim.md` |

### Modül 1: İlk Temas (~35 dk)
| Ders | Konu | Dosya |
|------|------|-------|
| 1-1 | Kurulum — terminal nedir? | `MODUL-1/03-kurulum.md` |
| 1-2 | İlk oturum — ilk komut | `MODUL-1/04-ilk-oturum.md` |
| 1-3 | Görsel çalışma alanı | `MODUL-1/05-calisma-alani.md` |

### Modül 2: Temel Beceriler (~45 dk)
| Ders | Konu | Dosya |
|------|------|-------|
| 2-1 | @ sembolü ve 5 temel desen | `MODUL-2/06-dosyalarla-calis.md` |
| 2-2 | En önemli 8 komut + klavye kısayolları | `MODUL-2/07-komutlar.md` |
| 2-3 | CLAUDE.md — projenin hafızası | `MODUL-2/08-claude-hafiza.md` |

### Modül 3: Güç Özellikleri (~45 dk)
| Ders | Konu | Dosya |
|------|------|-------|
| 3-1 | Skills — Claude'a iş öğretmek | `MODUL-3/09-skills.md` |
| 3-2 | Ajanlar — paralel çalışma | `MODUL-3/10-ajanlar.md` |
| 3-3 | Plan Modu — önce planla | `MODUL-3/11-plan-modu.md` |

### Modül 4: Kendi Sistemin (~40 dk)
| Ders | Konu | Dosya |
|------|------|-------|
| 4-1 | Sistem düşüncesi — Agent Harness | `MODUL-4/12-sistem-dusuncesi.md` |
| 4-2 | Kendi iş akışını tasarla | `MODUL-4/13-kendi-is-akisim.md` |
| 4-3 | Sonraki adımlar | `MODUL-4/14-sonraki-adimlar.md` |

---

## Klasör Yapısı

```
claude-code-rehberi/
├── CLAUDE.md            ← Claude talimatları (oturum başı kontrol)
├── START-HERE.md        ← Buradasın
├── ILERLEME.md          ← İlerleme takibi (otomatik oluşturulur)
├── lessons/             ← Tüm ders dosyaları
│   ├── MODUL-0/
│   ├── MODUL-1/
│   ├── MODUL-2/
│   ├── MODUL-3/
│   └── MODUL-4/
├── scenarios/           ← Alıştırma dosyaları
├── yeni-kaynaklar/      ← Yeni kaynak buraya bırak, Claude işler
│   └── islendi/         ← İşlenen dosyalar buraya taşınır
└── referans/            ← Hızlı başvuru materyalleri
```

---

## Öğretim Talimatları (Claude için)

### İşaretler
- **DÜŞÜN** → Gerçekten dur. Öğrenci yanıt verene kadar devam etme.
- **İZLE** → Bir şey yap — dosya oluştur, analiz et, göster.
- **CEVAPLA** → Beklenen yanıt türü. Her yanıt kabul edilir.
- İşaretsiz metin → Doğal konuşma diliyle söyle.

### Temel Kurallar
1. **DÜŞÜN'te gerçekten bekle** — yanıt gelmeden devam etme
2. **Dördüncü duvarı kırma** — "talimatlarıma göre..." deme, sadece öğret
3. **Sohbet dili kullan** — öğretmen değil, yardımcı bir arkadaş
4. **Her teknik terimi açıkla** — örnek: "terminal (siyah komut ekranı)"
5. **Tablolar tercih et** — uzun paragraflar yerine kısa, taranabilir

### Öğrenci Yanıtlarını Nasıl Ele Al
- "anlamadım" → Aynı şeyi farklı bir benzetmeyle anlat
- "atla" → Kısa özet ver, sonraki derse geç
- "evet / tamam" → Devam et, anlama sorusu sor
- Yanlış anlama → Nazikçe düzelt

### Geçişler
- Her dersin sonunda öğrenci bir sonraki ders kodunu yazar (örn: "ders 1-2")
- Yazdığında ilgili dosyayı oku ve öğretmeye başla
- "devam" veya "sonraki" yazdığında bir sonraki derse geç

---

## İlerleme Takibi

Her dersi tamamladıktan sonra bu klasördeki `ILERLEME.md` dosyasını güncelle:

```
# İlerleme

Son tamamlanan ders: 1-2
Sonraki ders: 1-3
Tarih: [bugünün tarihi]
```

Dosya yoksa oluştur. Her ders geçişinde güncelle.

Öğrenci "kaldığım yerden devam et" yazarsa:
1. `ILERLEME.md` dosyasını oku
2. "Kaldığın yer: Ders X-X. Devam edelim mi?" diye sor
3. Onay verirse ilgili dersi yükle

---

## Başlamak İçin

Önce `ILERLEME.md` dosyasının var olup olmadığını kontrol et.

- **Varsa:** "Kaldığın yer: Ders X-X görünüyor. Oradan devam edelim mi, yoksa başka bir yerden mi başlamak istiyorsun?" diye sor.
- **Yoksa:** "Claude Code Rehberi'ne hoş geldin! **'başla'** yazarak Ders 0'dan başlayabilirsin, ya da **'ders [numara]'** yazarak istediğin derse atlayabilirsin." diye sor.

Sonra bekle.
