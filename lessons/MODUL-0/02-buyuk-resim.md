# Ders 0-2: Büyük Resim

Claude Code'u bir sohbet penceresi gibi görüyorsak — anlayamayız.

Onu bir **işletim sistemi** gibi görmeliyiz.

---

DÜŞÜN: Bir şirkette sekreter ne yapar? Direktör ne yapar? İkisi arasındaki fark nedir?

CEVAPLA: [Kendi yorumunu paylaşır]

---

Tam. Sekreter söyleneni yapar. Direktör sistemi tasarlar ve yönetir.

Claude Code'da sen direktörsün. Claude Code da hem direktörün sağ kolu hem de şirketin işletim sistemi.

---

## Claude Code'un Katman Haritası

```
SEN
(direktör — ne yapılacağına karar veriyorsun)
    ↓
CLAUDE CODE
(asistan + işletim sistemi — nasıl yapılacağını buluyor)
    │
    ├── Dosya Sistemi
    │   Bilgisayarındaki klasörler, dosyalar.
    │   Claude okur, yazar, düzenler, siler.
    │
    ├── Skills (Beceriler)
    │   Claude'a öğrettiğin özel talimatlar.
    │   Örnek: "Toplantı notlarını şu formatta özetle"
    │
    ├── CLAUDE.md (Kalıcı Hafıza)
    │   Her oturumda Claude'un okuduğu brifing belgesi.
    │   "Sen kimsin, nasıl çalışıyoruz, kurallarımız neler."
    │
    └── MCP Bağlantıları (Dış Sistemler)
        Google, Notion, Slack, veritabanları...
        Claude bunlara da erişebilir — izin verirsen.
```

---

DÜŞÜN: Bu haritada seni en çok ilgilendiren katman hangisi? Neden?

CEVAPLA: [Bir katmanı seçer]

---

Seçimin mantıklı. Her katmanı ilerleyen derslerde bizzat kullanacağız.

Şimdi çok önemli bir şeyi söyleyeyim:

**Terminal (siyah ekran) sadece konuşma yeridir.**

Claude ile nasıl konuştuğun terminalden görünür. Ama asıl iş arka planda, dosyalarda olup bitiyor.

Yani şunu gördüğünde:

```
> Bu klasördeki dosyaları organize et.
```

Claude terminalde cevap verir ama asıl iş — dosyaları taşımak, yeniden adlandırmak, klasörler oluşturmak — dosya sisteminde gerçekleşir.

Bunu anlamak kritik. Çünkü çıktı terminalde değil, klasörde görünür.

---

DÜŞÜN: "Terminal sadece konuşma yeri" fikrini kendi cümlelerinle açıklar mısın?

CEVAPLA: [Kendi yorumunu paylaşır — anladıysa tebrik, anlamadıysa farklı örnekle tekrar]

---

Modül 0 tamamlandı.

Şu ana kadar şunları gördün:

| Ders | Kazanım |
|------|---------|
| 0-0 | Kursun DÜŞÜN/İZLE/CEVAPLA formatını anladın |
| 0-1 | ChatGPT ile Claude Code arasındaki temel farkı gördün |
| 0-2 | Claude Code'un katman haritasını kafanda canlandırdın |

Bunlar **Bloom Taksonomisi**nde "Hatırla" ve "Anla" seviyesi. Yani temel anlayış.

Modül 1'de artık **yapacağız** — kurulum, ilk komut, ilk sonuç.

---

**Öğrendiklerin:**
- Sen direktörsün, Claude Code işletim sistemi
- 4 katman: Dosyalar, Skills, Hafıza (CLAUDE.md), Bağlantılar
- Terminal konuşma yeri — asıl iş dosyalarda olur

**Sırada ne var:** Modül 1 — Claude Code'u gerçekten kurup açıyoruz.

**Devam etmek için:** "modül 1" veya "ders 1-1" yaz
