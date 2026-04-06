# Ders 4-2: Kendi İş Akışını Tasarla

Bu derste bir şey üreteceksin.

Sadece okumak değil — kendi sisteminizi kurmak.

---

DÜŞÜN: Şu an düzenli tekrar eden 3 işini yaz. (Haftalık rapor? Müşteri özeti? İçerik taslağı? Ne olursa olsun.)

CEVAPLA: [3 iş listeler]

---

Bu 3 iş senin **skill kütüphanenin** temeli olacak.

---

## İkinci Beyin Klasörü

Walid Chaar adlı bir içerik üreticisi Claude Code'u şöyle kullanıyor:

```
ikinci-beynim/
│
├── CLAUDE.md              ← "Ben kimim, nasıl çalışıyoruz"
│
├── 00_Inbox/              ← Hızlı yakalama
│   "Şimdi düşündüm, sonra işleyeceğim"
│
├── 01_Projeler/           ← Aktif işler
│   Her projenin kendi klasörü
│
├── 02_Alanlar/            ← Süregelen konular
│   İş, sağlık, öğrenme, finans...
│
├── 03_Kaynaklar/          ← Referans materyaller
│   Kitaplar, makaleler, notlar
│
└── 04_Arsiv/              ← Tamamlanan işler
    Bitti ama silinmeyecek
```

Bu yapı PARA sistemi olarak bilinir (Projects / Areas / Resources / Archive).

Claude bu yapıyı bildiğinde "yeni not al" dediğinde nereye koyacağını bilir.

---

DÜŞÜN: Bu 5 klasörü kendi iş hayatınla eşleştir. Her birine bir örnek yaz.

CEVAPLA: [Her klasör için bir örnek verir]

---

## Sistemi Kur

İZLE: Kullanıcının seçtiği bir çalışma klasörüne bu yapıyı kur:
- `ikinci-beynim/` ana klasörü
- 5 alt klasör (00_Inbox, 01_Projeler, 02_Alanlar, 03_Kaynaklar, 04_Arsiv)
- Her klasörde kısa bir `README.md` (bu klasör ne içindir)
- Ana klasörde temel bir `CLAUDE.md` taslağı

---

DÜŞÜN: Klasörler oluştu mu? README dosyalarına baktın mı?

CEVAPLA: [Gördüğünü paylaşır]

---

## Skill Kütüphanesini Başlat

Hatırlıyor musun? Dersin başında 3 tekrar eden iş yazmıştın.

Şimdi en öncelikli olanı için bir skill yazacağız.

İZLE: Kullanıcının listelediği 3 işten ilkini seç. `.claude/skills/` altında ona özel bir SKILL.md oluştur. Adımları kullanıcıyla birlikte netleştir.

---

DÜŞÜN: Oluşturulan skill'e bak. Adımlar doğru mu? Eksik bir şey var mı?

CEVAPLA: [Değerlendirir, gerekirse düzeltmeler söyler]

---

İZLE: Gerekli düzeltmeleri yap.

---

## Çalışma Ritmi

İyi bir Claude Code kullanıcısı nasıl çalışır?

```
Sabah         → Claude Code'u aç, CLAUDE.md otomatik yüklenir
                 "Bugün ne var?" sorusunu sor

Gün içinde    → Görevleri delege et, sonuçları gözden geçir
                 Yeni skills ekle, eskilerini güncelle

Hafta sonu    → Tamamlanan işleri 04_Arsiv'e taşı
                 CLAUDE.md'yi güncelle
                 Yeni skill fırsatlarını belirle
```

---

DÜŞÜN: Bu ritimden kendi çalışma alışkanlıklarınla uyumlu olanlar neler?

CEVAPLA: [Değerlendirmesini paylaşır]

---

## Sistemin Büyüdükçe

Zaman içinde skill kütüphanen büyüyecek.

```
.claude/skills/
├── haftalik-rapor/
├── musteri-ozeti/
├── icerik-taslagi/
├── toplanti-notu/
├── veri-analizi/
└── ... (her ay birkaç yeni skill eklenecek)
```

Her skill = tekrar eden bir işten kurtulmak.

3 ayda 15-20 skill kütüphanesi olduğunda geriye döner bakarsın ve "bunu nasıl yaşıyordum?" diye soracaksın.

---

**Öğrendiklerin:**
- İkinci Beyin yapısı: Inbox / Projeler / Alanlar / Kaynaklar / Arşiv
- Skill kütüphanesi tekrar eden her işten kurtarır
- Çalışma ritmi sabah rutini + gün içi delegasyon + haftalık bakım

**Sırada ne var:** Son ders — nereye gidebilirsin? MCP bağlantıları, tarayıcı otomasyonu, gelişmiş ajanlar.

**Devam etmek için:** "ders 4-3" yaz
