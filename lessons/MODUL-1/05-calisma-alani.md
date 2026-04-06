# Ders 1-3: Görsel Çalışma Alanı

Şu an terminalde Claude Code ile konuşuyorsun.

Ama bir sorun var: dosyaların nerede, ne olduğunu göremiyorsun.

---

DÜŞÜN: Ders 1-2'de dosyalar taşındığında klasörü görmek için ne yaptın? Terminal dışına çıkmak zorunda kaldın mı?

CEVAPLA: [Evet / hayır / ne yaptığını anlatır]

---

Terminal'de konuşuyorsun ama dosyalar göremiyorsun. Kör uçmak gibi.

Çözüm: **çift panel**.

Sol tarafta Claude Code (terminal). Sağ tarafta dosyaların.

---

## Seçenekler

İki yol var:

| Araç | Nasıl | Uygunluk |
|------|-------|---------|
| **VS Code + Claude uzantısı** | Ücretsiz kod editörü, Claude entegrasyonu var | Önerilen — en çok özellik |
| **Nimbalyst** | Claude Code için özel uygulama | Terminal görmek istemeyenler için |

VS Code ile devam ediyoruz. (Nimbalyst'i de deneyebilirsin — bağlantı dersin sonunda.)

---

## VS Code Kurulumu

**Adım 1 — VS Code indir:**

code.visualstudio.com adresine git → İşletim sistemine uygun versiyonu indir → Kur.

**Adım 2 — Claude Code uzantısını kur:**

VS Code açıldığında sol taraftaki panel simgelerinden **Extensions** (blok simgesi) tıkla.

Arama kutusuna "Claude Code" yaz.

Anthropic tarafından yayınlanmış uzantıyı bul → **Install**.

**Adım 3 — Claude Code'u VS Code'dan başlat:**

VS Code'un alt kısmında bir terminal paneli var (View → Terminal).

Bu terminale `claude` yaz — artık VS Code içinden çalışıyor.

---

DÜŞÜN: VS Code açık mı? Sol tarafta dosya ağacını, altta terminali görebiliyor musun?

CEVAPLA: Evet / Hayır / Nerede arayacağımı bilmiyorum

---

Göremediysen: View menüsü → Explorer (dosya ağacı) ve View → Terminal.

---

## Çift Panel'in Gücü

Artık şöyle çalışacaksın:

```
Sol: Dosya ağacı          |  Sağ/Alt: Terminal (Claude Code)
─────────────────────────────────────────────────
📁 projelerim/           |  > Bu klasörü organize et.
  📁 raporlar/           |
  📁 sunumlar/           |  [Claude çalışıyor...]
  📁 notlar/             |
  📄 CLAUDE.md           |  Hazır. 8 dosya 3 klasöre taşındı.
```

Claude terminalde çalışırken sol tarafta dosyaların hareket ettiğini canlı görebilirsin.

---

DÜŞÜN: Ders 1-2'de yaptığımız dosya organizasyonunu şimdi VS Code sol panelinden bulabildin mi?

CEVAPLA: Evet / Hayır

---

## Bypass Permissions: Onay Yorgunluğunu Bitir

Çift panel kurulduktan sonra fark edebilirsin: Claude her küçük adımda soru soruyor.

"Bu dosyayı okuyabilir miyim?" "Bunu yapabilir miyim?" "Silmeli miyim?"

İlk başta faydalı. Ama zamanla yavaşlatır.

**Bypass Permissions** bu onayları kapatır — Claude işi bitirene kadar beklemeden devam eder.

Nasıl açılır (VS Code):

| Adım | Yapılacak |
|------|-----------|
| 1 | Sol panelde Extensions (blok simgesi) tıkla |
| 2 | Kurulu uzantılar arasında Claude Code'u bul |
| 3 | Ayarlar (dişli) → "Bypass Permissions" seçeneğini aktif et |

---

DÜŞÜN: Bu ayarı buldun mu? Açıp kapatabildin mi?

CEVAPLA: Evet / Hayır / Nerede olduğunu bulamadım

---

> **Ne Zaman Açmalı?**
> - **Açık tut:** Tekrar eden, güvendiğin işler (dosya organize, metin özetle)
> - **Kapalı tut:** İlk kez yaptığın büyük işler — her adımı görmek, neyi onayladığını anlamak için

Bu ayar, bir sonraki derste öğreneceğin **Auto-Accept modunun** VS Code versiyonudur. İkisi aynı mantıkta çalışır.

---

## Nimbalyst (Alternatif)

Terminal görmek istemiyorsan Nimbalyst daha temiz bir arayüz sunuyor.

nimbalyst.com adresinden indirebilirsin. Claude hesabınla giriş yapıyorsun, terminal görmeden çalışıyorsun.

Dezavantajı: bazı ileri özellikler terminal gerektiriyor.

Şimdilik VS Code ile devam etmeni öneririm.

---

**Öğrendiklerin:**
- Terminal tek başına kör uçmak gibi — dosyaları görmek gerekiyor
- VS Code + Claude uzantısı = çift panel çalışma alanı
- Dosyalar hareket ederken canlı izleyebiliyorsun

**Sırada ne var:** Modül 2 — gerçek dosyalarla çalışmaya başlıyoruz. @ sembolü, 5 temel desen, ve CLAUDE.md.

**Devam etmek için:** "modül 2" veya "ders 2-1" yaz

---

> **Not:** Nimbalyst için nimbalyst.com — VS Code Claude uzantısı için VS Code Marketplace'de "Claude Code" ara.
