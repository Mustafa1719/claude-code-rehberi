# Claude Code — Hızlı Referans Kartı

*Bu kartı yanında tut. Unuttuğunda buraya bak.*

---

## Temel Komutlar

| Komut | Ne Yapar |
|-------|---------|
| `claude` | Claude Code'u başlat |
| `claude --version` | Versiyon kontrolü |
| `/help` | Tüm komutları listele |
| `/plan` | Plan modu — önce planla |
| `/init` | CLAUDE.md otomatik oluştur |
| `/context` | Bağlam kullanımını göster |
| `/compact` | Oturumu sıkıştır, yer aç |
| `/clear` | Her şeyi sil, sıfırla |
| `/model` | Modeli değiştir |
| `/rewind` | Son işlemi geri al |

---

## Çalışma Modları

| Mod | Giriş | Ne Yapar |
|-----|-------|---------|
| **Normal** | Varsayılan | Her önemli adımda onay ister |
| **Auto-Accept** | `Shift+Tab` × 1 | Otomatik devam eder |
| **Plan Modu** | `Shift+Tab` × 2 veya `/plan` | Sadece planlar, dokunmaz |
| **Geri dön** | `Esc` | Normal moda dön |

---

## Klavye Kısayolları

### Oturum

| Ortam | Başlatma | Kapatma |
|-------|---------|---------|
| **Terminal** | `claude` | `/exit` veya `Ctrl+C` |
| **VS Code eklentisi** | Panel açık | Sohbet panelini kapat (X) |

| Kısayol / Komut | Ne Yapar | Nerede |
|----------------|---------|--------|
| `claude` | Yeni oturum başlat | Terminal |
| `/exit` | Claude Code'dan çık | Terminal |
| `Ctrl + C` | Çalışan işi durdur | Terminal |
| `Ctrl + C` (2 kez) | Oturumu kapat | Terminal |

> Ayar değişikliği yaptıysan → oturumu kapat → yeniden aç

### Gezinme ve Düzenleme

| Kısayol | Ne Yapar |
|---------|---------|
| `↑` / `↓` | Komut geçmişinde gezin |
| `Ctrl + R` | Komut geçmişinde ara |
| `Ctrl + L` | Terminal ekranını temizle |
| `Ctrl + V` | Görüntü veya metin yapıştır |
| `Esc` | Claude'u durdur / moda geri dön |

---

## Dosya Referanslama

```
@dosya.txt           → tek dosya
@klasor/             → tüm klasör
@klasor/dosya.txt    → belirli dosya
Ctrl+V               → ekran görüntüsü yapıştır
```

---

## 5 Temel Desen

| # | Desen | Örnek |
|---|-------|-------|
| 1 | Tek Dosya → Çıkar | `@not.txt görevleri listele` |
| 2 | Klasör → Sentezle | `@musteriler/ ortak sorunları bul` |
| 3 | Şablon Uygula | `@veri.txt haftalık rapor formatına dök` |
| 4 | Görsel → Analiz | Yapıştır → "Bu görseldeki metni çıkar" |
| 5 | Web → Araştır | "Bu konuyu araştır ve özetle" |

---

## Delegasyon Formülü

```
NE istiyorum  +  NASIL bir sonuç bekliyorum
```

❌ "Bu dosyaları nasıl organize etmeliyim?"
✅ "Bu dosyaları organize et — tarih ve konuya göre."

---

## CLAUDE.md Şablonu

```markdown
## Ben Kimim
- Dil: Türkçe
- Alan: [iş alanın]

## Çalışma Kuralları
- Değişiklik öncesi sor
- Kısa cevap, madde işareti tercih ederim

## Asla Yapma
- [hassas klasörler]
- İzinsiz dosya silme

## Her Zaman Yap
- Türkçe cevap ver
- Büyük görevlerde önce plan göster
```

---

## Skill Klasörü Yapısı

```
.claude/
└── skills/
    └── skill-adi/
        └── SKILL.md
```

Çağırmak: `/skill-adi`

---

## İkinci Beyin Klasör Yapısı

```
ikinci-beynim/
├── CLAUDE.md
├── 00_Inbox/       ← hızlı yakalama
├── 01_Projeler/    ← aktif işler
├── 02_Alanlar/     ← süregelen konular
├── 03_Kaynaklar/   ← referanslar
└── 04_Arsiv/       ← tamamlananlar
```

---

## Ajan Kullanımı

**Paralel çalışma için:**
```
Bu 20 dosyayı paralel olarak analiz et.
Her birinden [X]'i çıkar. Sonunda birleştir.
```

**Danışman ekibi için:**
```
Bu kararı 3 farklı perspektiften değerlendir:
1. Finansal açıdan
2. Müşteri açısından
3. Operasyonel açıdan
```

---

## MCP Bağlantısı (İleri Seviye)

```json
"mcpServers": {
  "araç-adi": {
    "command": "npx",
    "args": ["-y", "@paket/adi"],
    "env": { "API_KEY": "..." }
  }
}
```

Dosya: `~/.claude/settings.json`

---

*Tam kurs: `START-HERE.md` | Tam kaynaklar: `referans/kaynak-listesi.md`*
