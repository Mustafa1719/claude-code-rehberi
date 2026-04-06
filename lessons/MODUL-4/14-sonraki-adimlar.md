# Ders 4-3: Sonraki Adımlar

Bu kursun başında Claude Code hakkında ne biliyordun?

---

DÜŞÜN: Bu kursu almadan önceki kendinle şimdiki kendin arasında ne değişti? En büyük fark neydi?

CEVAPLA: [Dürüst bir değerlendirme yapar]

---

## Ne Öğrendin?

5 modülde öğrendiklerin:

| Modül | Kazanım |
|-------|---------|
| **0** | ChatGPT "anlatır", Claude Code "yapar" — farkı gördün |
| **1** | Kurulum, terminal, ilk delegasyon — elimle yaptın |
| **2** | @ sembolü, 8 komut, CLAUDE.md — gerçek dosyalarda çalıştın |
| **3** | Skills, ajanlar, Plan Modu — tekrar eden işleri otomatikleştirdin |
| **4** | Sistem tasarımı, ikinci beyin, kendi skill kütüphaneni başlattın |

Bu Bloom Taksonomisinin tüm basamakları:
```
Hatırla → Anla → Uygula → Analiz et → Değerlendir → Yarat
```

Sen artık sadece kullanıcı değilsin. Sistem tasarımcısısın.

---

## Bundan Sonra Öğrenebileceklerin

Daha derin gitmek istersen:

| Konu | Ne Yapar | Zorluk |
|------|---------|--------|
| **MCP Sunucuları** | Google Drive, Notion, Slack, GitHub'a Claude'u bağla | Orta |
| **Tarayıcı Otomasyonu** | Claude web sitelerinde gezinsin, form doldursun | Orta |
| **Custom Sub-Agents** | Her biri farklı uzmanlıkta 4-5 danışman ajanı kur | İleri |
| **Hooks** | Her işlem sonrası otomatik kalite kontrolü | İleri |
| **Playwright ile Test** | Otomatik web testi yaptır | İleri |

---

DÜŞÜN: Bu listeden sıradaki öğrenmek istediğin şey hangisi? Neden?

CEVAPLA: [Bir konu seçer]

---

## MCP'ye Yakın Bakış

MCP (Model Context Protocol) = Claude'u dış sistemlere bağlayan standart.

Kurulunca şunları yapabilirsin:

```
"Google Drive'ımdaki son 10 dokümanı özetle"
"Notion'daki görev listemi güncelle"
"GitHub'da yeni bir issue aç"
"Takvimime yarın 10:00'a toplantı ekle"
```

Nasıl kurulur: CLAUDE.md'deki MCP Kurulumu bölümüne bak veya:
`referans/kaynak-listesi.md` → MCP Sunucuları başlığı

---

## Topluluk ve Kaynaklar

Öğrenmeye devam etmek için:

| Kaynak | Ne İçin |
|--------|---------|
| **ccforeveryone.com** | Kapsamlı Claude Code rehberi (İngilizce) |
| **claude.ai/docs** | Resmi Anthropic dökümantasyonu |
| **X (Twitter)** | #ClaudeCode — gerçek kullanım örnekleri |
| **referans/cheat-sheet-ozet.md** | Bu kursun hızlı referans kartı |

---

## WAT Framework: Sistemi Anlamak İçin 3 Kavram

Uzmanlar Claude Code'u anlatırken üç İngilizce kelime kullanır: **W**orkflow, **A**gent, **T**ool.

| Kavram | Türkçe | Ne Demek |
|--------|--------|---------|
| **Workflow** | İş Akışı | Baştan sona otomatik çalışan süreç |
| **Agent** | Ajan | Bağımsız karar veren, görevi yürüten yardımcı |
| **Tool** | Araç | Claude'un bağlandığı dış sistem (Gmail, Apify, Drive…) |

Bunlar birleşince ne olur?

```
"Gmail'den gelen şikayetleri oku (Tool)
 → Her biri için çözüm öner (Agent)
 → Hepsini tek raporda topla (Workflow)"
```

Bu üç kavramı bilmek, Claude Code topluluğunu, dökümanları ve ileri kaynakları anlamayı kolaylaştırır.

---

## Büyük Projeye Doğru Başlamak: .md Metodolojisi

Claude Code'a doğrudan "şunu yap" demek işe yarar. Ama büyük projelerde daha güvenilir bir yöntem var:

**Adım 1 — Claude.ai'da planla:**
```
claude.ai'ı aç → Projeyi tarif et →
"Bunu Claude Code'a verebileceğim bir .md dosyası hazırla" de
```

**Adım 2 — .md dosyasını indir, klasöre at**

**Adım 3 — Claude Code'a ver:**
```
Bu proje dosyasını oku ve başlayalım
```

Farkı nedir? Claude Code, işi başlatmadan önce hedefi, araçları ve dosya yapısını biliyor. Rastgele karar vermiyor — planı takip ediyor.

> Bu, bir şefe önceden menüyü hazırlatmak gibi. Mutfağa girdiğinde ne pişireceğini biliyor.

---

## Canlıya Alma: Sistemini Buluta Taşı

Kurduğun sistemin sürekli çalışmasını istiyorsan — bilgisayarın kapalıyken bile:

| Platform | Ne İçin | Zorluk |
|----------|---------|--------|
| **Modal.com** | Python tabanlı otomasyonlar, zamanlı görevler | Orta |
| **Vercel** | Web uygulamaları (analiz_yz gibi) | Kolay |
| **n8n Cloud** | Workflow otomasyonları | Kolay |
| **GitHub Actions** | Kod tabanlı periyodik görevler | Orta |

Modal.com örneği: "Projeyi Modal üzerinde kur ve her gün saat 9'da çalışsın" → Claude kurulumu yapar, sistemi buluta taşır.

---

## Son Söz

Yapay zeka dünyasında iki grup var.

Birinci grup AI'a sorar. İkinci grup AI'a **yaptırır.**

Sen bu kursa başladığında terminale ilk kez baktın — ve korkmadın.

Şimdi dosyaları organize ediyorsun, skills yazıyorsun, ajanları paralel çalıştırıyorsun, kendi sistemini tasarlıyorsun.

Bu kursu tamamlayanların büyük çoğunluğu şunu söylüyor: "Birkaç haftada en az 5-10 saatlik işimi Claude'a devreddim."

Sen artık o grubun içindesin.

Fark skills'te değil, sistemde değil, modelde değil.

Fark bakış açısında.

"Bu işi nasıl yapayım?" yerine "Bu işi nasıl devredeyim?" diye sormaya başladığında — geçttin.

---

> Bu kursu **Mustafa Aydın** hazırladı.
> Sorularını, geri bildirimlerini ve deneyimlerini paylaşmaktan çekinme.
> [YouTube](https://www.youtube.com/@mustafa1aydin) · [LinkedIn](https://www.linkedin.com/in/mustafaaydin1/) · mustafaaydin@lab-mind.com

---

DÜŞÜN: Bu kurstan öğrendiklerini bu hafta gerçekten kullanacak mısın? Neyle başlayacaksın?

CEVAPLA: [Bir taahhüt verir]

---

**Tebrikler.**

`referans/cheat-sheet-ozet.md` dosyasını yanında tut. Komutları unutursan oraya bak.

Her yeni skill yazdığında, her otomasyonu kurduğunda, kursa geri dön — farklı göreceksin.

---

**Bu kursda öğrendiklerin:**
- Claude Code bir chatbot değil, bir işletim sistemi
- DÜŞÜN / İZLE / CEVAPLA — aktif öğrenme
- Skills, CLAUDE.md, ajanlar, Plan Modu
- Kendi sistemini tasarladın

**Kurs tamamlandı.**
Soru veya devam için: yeni bir oturumda `START-HERE.md dosyasını oku` yaz.
