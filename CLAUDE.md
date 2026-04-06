# CLAUDE.md

Bu dosya Claude Code'a bu klasörle nasıl çalışacağını anlatır.

---

## Oturum Başı Otomatik Kontrol

Her yeni oturumda şunu yap:

1. `yeni-kaynaklar/` klasörünü kontrol et (`islendi/` alt klasörü hariç)
2. İçinde dosya varsa her birini oku
3. Hangi modüle / derse ait olduğuna karar ver
4. Bana şu formatta göster:

```
📥 Yeni Kaynak Bulundu: [dosya adı]
→ İlgili Modül: Modül X — Ders Y
→ Eklenecek İçerik: [kısa özet]
→ Onaylıyor musun?
```

5. Onayımı aldıktan sonra ilgili ders dosyasını güncelle
6. İşlenen dosyayı `yeni-kaynaklar/islendi/` klasörüne taşı

Onaysız hiçbir ders dosyasını değiştirme.

---

## Klasör Yapısı

```
claude-code-rehberi/
├── CLAUDE.md              ← Buradasın (Claude talimatları)
├── START-HERE.md          ← Kursa buradan başla
├── ILERLEME.md            ← İlerleme takibi (otomatik oluşturulur)
├── lessons/               ← Ders dosyaları
│   ├── MODUL-0/           ← Neden Claude Code? (~20 dk)
│   ├── MODUL-1/           ← İlk temas (~35 dk)
│   ├── MODUL-2/           ← Temel beceriler (~45 dk)
│   ├── MODUL-3/           ← Güç özellikleri (~45 dk)
│   └── MODUL-4/           ← Kendi sistemin (~40 dk)
├── scenarios/             ← Alıştırma dosyaları
├── yeni-kaynaklar/        ← Yeni kaynak buraya bırakılır
│   ├── BENI-OKU.md        ← Kullanım talimatları
│   ├── islendi/           ← İşlenen dosyalar buraya taşınır
│   ├── modul-0/           ← (opsiyonel) modüle göre sınıflandır
│   ├── modul-1/
│   ├── modul-2/
│   ├── modul-3/
│   └── modul-4/
├── referans/              ← Hızlı başvuru materyalleri
└── .claude/               ← Claude Code yapılandırması
    ├── commands/          ← Slash komutları
    └── skills/            ← Öğretim scriptleri
```

---

## Yeni Kaynak Nasıl Eklenir?

### Yöntem 1 — Sadece dosya bırak
Dosyayı `yeni-kaynaklar/` klasörüne koy. Claude hangi modüle ait olduğuna kendisi karar verir.

### Yöntem 2 — Alt klasörle belirt (daha hızlı)
```
yeni-kaynaklar/
└── modul-3/    ← "Bu Modül 3 için" demek
    └── yeni-makale.pdf
```

### Yöntem 3 — Meta dosyayla not bırak
```
yeni-kaynaklar/
├── kaynak.pdf
└── kaynak.pdf.meta.txt   ← "Modül 2 komutlar dersine ekle"
```

---

## Modül Referansı

| Modül | Konu | Klasör |
|-------|------|--------|
| 0 | Neden Claude Code? | `lessons/MODUL-0/` |
| 1 | Kurulum & İlk Temas | `lessons/MODUL-1/` |
| 2 | Temel Beceriler | `lessons/MODUL-2/` |
| 3 | Güç Özellikleri | `lessons/MODUL-3/` |
| 4 | Kendi Sistemin | `lessons/MODUL-4/` |
