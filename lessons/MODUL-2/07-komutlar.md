# Ders 2-2: Temel Komutlar

Claude Code'da 62'den fazla komut var.

Hepsini ezberlemene gerek yok. Zaten kullanmayacağın çoğunu.

Ama 8 tanesini bilirsen, %90 işini halledersin.

---

DÜŞÜN: `/help` yaz ve çıkan listeye bir bak. Kaç komut görüyorsun?

CEVAPLA: [Sayıyı söyler]

---

Evet, çok fazla. Ama korkulacak bir şey değil.

Araba kullanmayı öğrenirken motorun kaç parçadan oluştuğunu öğrenmezsin. Direksiyonu, gazı, freni öğrenirsin.

Biz de öyle yapacağız.

---

## 8 Kritik Komut

| Komut | Ne Yapar | Ne Zaman Kullanırsın |
|-------|---------|---------------------|
| `/plan` | Önce plan yap, sonra çalış | Karmaşık veya büyük görevlerde |
| `/context` | Ne kadar "alan" kaldığını göster | Uzun oturumlarda yer kontrolü |
| `/compact` | Oturumu sıkıştır, alan aç | Bağlam dolmaya başladığında |
| `/clear` | Her şeyi sil, sıfırdan başla | Yeni bir konuya geçerken |
| `/init` | CLAUDE.md dosyasını otomatik oluştur | Yeni proje başlatırken |
| `/review` | Kod incelemesi yap — detaylı analiz | Bir şeyi paylaşmadan önce |
| `/cost` | Bu oturumda ne kadar harcandığını göster | Maliyet takibi |
| `/resume` | Son oturumda kaldığın yerden devam et | Yarım kalan işe dönünce |
| `/btw` | Mevcut işi bölmeden araya soru sor | Konuyu değiştirmeden ek soru |
| `/rewind` | Son işlemi geri al | Hata yaptığında |
| `/help` | Tüm komutları listele | Bir komut aradığında |

---

DÜŞÜN: Bu 8 komuttan hangisi sana en mantıklı geldi? Hangisini bugün kullanırdın?

CEVAPLA: [Bir komut seçer]

---

## 3 Çalışma Modu

Komutlardan daha önemli bir kavram: **mod**.

Claude Code 3 farklı modda çalışabilir:

| Mod | Nasıl Çalışır | Ne Zaman Kullan |
|-----|--------------|----------------|
| **Normal** (varsayılan) | Her önemli adımda senden onay ister | Dikkat gerektiren işler, ilk kez yaptığın şeyler |
| **Auto-Accept** | Onay beklemeden devam eder | Güvendiğin, tekrarlayan işler |
| **Plan Modu** | Sadece planlar, hiçbir şeye dokunmaz | Karmaşık görevler, büyük değişiklikler öncesi |

Geçiş:
- Normal → Auto-Accept: `Shift + Tab` (bir kez)
- Normal → Plan Modu: `Shift + Tab` (iki kez)
- Geri dönmek: `Esc`

---

DÜŞÜN: Hangi modda çalışmayı tercih ederdin? Neden?

CEVAPLA: [Yorumunu paylaşır]

---

İpucu: Yeni bir şey denerken **Normal mod** kullan. Claude senden onay ister, her adımı görürsün.

İş akışını öğrendikten sonra **Auto-Accept**'e geçebilirsin.

---

## Klavye Kısayolları

Mouse kullanmadan hızlı hareket etmeni sağlar. Bunları bir kez öğrenince çok işine yarar.

### Oturum Yönetimi

Kullandığın araca göre farklı çalışır:

| Ortam | Başlatma | Kapatma |
|-------|---------|---------|
| **Terminal** | `claude` yaz | `/exit` veya `Ctrl + C` |
| **VS Code eklentisi** | Panel zaten açık | Sohbet panelini kapat (X) |

| Kısayol / Komut | Ne Yapar | Nerede Çalışır |
|----------------|---------|---------------|
| `claude` | Yeni oturum başlat | Terminal |
| `/exit` | Claude Code'dan çık | Terminal |
| `Ctrl + C` | Claude'u durdur — işi yarıda kes | Terminal |
| `Ctrl + C` (iki kez) | Oturumu tamamen kapat | Terminal |

> **Önemli:** Bir ayar değiştirdiysen (hook, CLAUDE.md gibi) ve etkili olmasını istiyorsan oturumu kapatıp yeniden aç. Değişiklikler yeni oturumda devreye girer.

### Mod Geçişleri

| Kısayol | Ne Yapar |
|---------|---------|
| `Shift + Tab` (1 kez) | Normal → Auto-Accept moduna geç |
| `Shift + Tab` (2 kez) | Normal → Plan Moduna geç |
| `Esc` | İstediğin moda geri dön / Claude'u durdur |

### Metin ve Gezinme

| Kısayol | Ne Yapar |
|---------|---------|
| `↑` (yukarı ok) | Önceki komutu getir |
| `↑↑↑` (birkaç kez) | Komut geçmişinde geri git |
| `Ctrl + R` | Komut geçmişinde ara (bash) |
| `Ctrl + L` | Terminal ekranını temizle (Claude kapanmaz) |
| `Ctrl + V` | Ekran görüntüsü veya metin yapıştır |

### Yanıt Kontrolü

| Kısayol | Ne Yapar |
|---------|---------|
| `Esc` | Claude yazarken durdur, düzenle |
| `/rewind` | Son işlemi geri al |
| `/clear` | Konuşmayı sıfırla, yeni sayfadan başla |

---

DÜŞÜN: `/context` ve `/compact` komutlarını çalıştırdın mı? Ne değişti?

CEVAPLA: [Gözlemini paylaşır]

---

## Paylaşmadan Önce: /security-review

8 komutun ötesinde, bir tane daha var. Ama bu seni korumak için:

```
/security-review
```

Ne yapar? Kodun veya projenin içinde açıkta kalmış API anahtarı, şifre veya güvenlik açığı olup olmadığını tarar. Bulursa gösterir, düzeltir.

**Ne Zaman Kullanılır?**

```
Bir projeyi paylaşmadan önce          → /security-review
GitHub'a yüklemeden önce              → /security-review
Bir iş arkadaşına göndermeden önce   → /security-review
```

**Altın Kural:** API anahtarlarını hiçbir zaman doğrudan koda yazma.

Claude'a şunu söyle: *"Environment dosyası oluştur, API anahtarımı oraya koy."*

```
# ✅ Doğru
API_KEY=.env dosyasından okunur

# ❌ Yanlış
api_key = "sk-abc123..."  ← Kod içinde açık — tehlikeli
```

Bu kural küçük görünür ama projeyi paylaştığında anahtarın çalınmasını önler.

---

DÜŞÜN: `/security-review` komutunu aktif bir projende çalıştırdın mı? Ne buldu?

CEVAPLA: [Sonucu paylaşır — "temiz" de olur, bir uyarı da]

---

## Pratik: İki Komut + Bir Kısayol Dene

Şunları sırayla dene:

```
/context
```
Context penceresinin ne kadar dolduğunu göreceksin.

```
/compact
```
Oturum sıkıştırılır. Yer açılır.

Sonra `↑` tuşuna bas — az önce yazdığın komutu tekrar göreceksin.

---

DÜŞÜN: `↑` tuşu çalıştı mı? Bu kısayollardan hangisi sana en faydalı geldi?

CEVAPLA: [Gözlemini paylaşır]

---

**Öğrendiklerin:**
- 62 komut var ama 11 tanesi %90 işini görür
- 3 mod: Normal / Auto-Accept / Plan
- `/exit` veya `Ctrl+C` ile oturumu kapat — ayarlar yeni oturumda devreye girer
- `↑` geçmiş komutu getirir, `Esc` Claude'u durdurur

**Sırada ne var:** CLAUDE.md — Claude'un kalıcı hafızası. Her oturumda seni tanıyan bir asistan.

**Devam etmek için:** "ders 2-3" yaz
