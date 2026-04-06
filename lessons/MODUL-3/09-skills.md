# Ders 3-1: Skills — Claude'a Öğretmek

Her hafta aynı işi yapıyorsun. Toplantı notu alıyorsun. Claude'a veriyorsun. Aynı formatı açıklıyorsun. Tekrar tekrar.

Ya Claude o formatı bir kez öğrense ve hep hatırlasa?

Skills tam olarak bu.

---

DÜŞÜN: Her hafta veya her ay tekrar yaptığın, sıkıcı bulduğun bir iş var mı?

CEVAPLA: [Bir iş tanımlar]

---

## 3 Seviye

Claude ile çalışmanın 3 seviyesi var:

| Seviye | Nasıl Çalışır | Sorun |
|--------|--------------|-------|
| **1 — Simple Chat** | Her seferinde açıklarsın | Tekrar tekrar aynı talimatı yazıyorsun |
| **2 — Skill** | Bir kez tanımlarsın, hep hatırlar | Sadece `/komut` yazmak yeterli |
| **3 — Plugin** | Skill + araçlar + otomasyon paketi | İleri seviye — şimdilik burada duralım |

Sen şu an muhtemelen Seviye 1'desin.

Skill öğrendikten sonra Seviye 2'ye geçeceksin.

---

DÜŞÜN: Şu an Seviye 1 misin? Yani her seferinde aynı talimatı mı yazıyorsun?

CEVAPLA: [Evet / Hayır / Ne demek istediğini anlıyorum]

---

## Skill Nedir?

Skill = Claude'a öğrettiğin, istediğinde çağırabileceğin özel talimat paketi.

Bir `.md` (markdown) dosyası. Ama özel bir klasörde:

```
.claude/
└── skills/
    └── toplanti-notu/
        └── SKILL.md
```

SKILL.md içinde şunlar olur:

```markdown
# Toplantı Notu Özeti

## Ne Yapar
Toplantı notlarını alır, görev listesine ve karar listesine dönüştürür.

## Nasıl Çağrılır
/toplanti-notu

## Adımlar
1. Notu oku
2. Görevleri listele (kişi + tarih ile)
3. Kararları listele
4. Katılımcıları listele
5. Çıktıyı Türkçe, madde işareti formatında sun
```

---

## İlk Skill'i Birlikte Yazalım

Klasik örnek: toplantı notu.

İZLE: `.claude/skills/toplanti-notu/` klasörü oluştur ve içine SKILL.md yaz. İçerik: toplantı notlarını görev listesi + karar listesi + katılımcı listesine dönüştüren Türkçe bir skill.

---

DÜŞÜN: Oluşturulan SKILL.md dosyasını gördün mü? Adımları mantıklı mı?

CEVAPLA: [Değerlendirmesini paylaşır]

---

## Skill'i Çağırmak

Skill'i kullanmak için terminale şunu yaz:

```
/toplanti-notu
```

Claude skill dosyasını okur ve o talimatlara göre çalışır.

Ardından notlarını yapıştır ya da `@dosya.txt` ile referans al.

---

## Kendi Skill'ini Yaz

Hatırladın mı? Dersin başında tekrar yaptığın bir iş söyledin.

Şimdi onun için bir skill yazmak istiyorsan:

İZLE: `scenarios/skill-olustur/` klasörünü aç. İçindeki yönlendirici soruları oku. Cevaplarına göre senin işin için bir SKILL.md birlikte oluşturalım.

---

DÜŞÜN: Oluşturulan skill'i `/skill-adi` yazarak dene. Ne oldu?

CEVAPLA: [Sonucu paylaşır]

---

## Sıfırdan Yazmak Zorunda Değilsin

Her skill'i baştan yazmak gerekmez. Başkalarının hazırladığı skill'leri de ekleyebilirsin.

Nasıl eklenir:

```
/ (slash) yaz → "manage plugins" seç → Skill URL'sini yapıştır → Ekle
```

Toplulukta hazır skill'ler var: video oluşturma, PDF işleme, web scraping, sunum hazırlama...

---

DÜŞÜN: Hazır bir skill olsa, hangi iş için kullanmak isterdin?

CEVAPLA: [Bir iş tanımlar — bu onların ideal skill'inin ipucu]

---

> **Kural:** Eğer bir işi 3+ kez kendin tanımladıysan → kendin yaz. Daha önce başkası yazdıysa → URL ile ekle. İkisi de aynı sonucu verir.

---

## Ne Zaman Skill Yazarsın?

```
Bir işi 3+ kez aynı şekilde yaptıysan → Skill zamanı
```

Örnekler:
- Haftalık durum raporu
- Müşteri maili şablonu
- İçerik taslağı
- Veri analiz formatı
- Toplantı özeti

---

**Öğrendiklerin:**
- Skills = Claude'a öğretilen kalıcı talimat paketleri
- `.claude/skills/` klasöründe SKILL.md olarak saklanır
- `/komut-adi` ile çağrılır
- Tekrar eden her iş için skill düşün

**Sırada ne var:** Ajanlar — paralel çalışma ile 10 katı hız.

**Devam etmek için:** "ders 3-2" yaz
