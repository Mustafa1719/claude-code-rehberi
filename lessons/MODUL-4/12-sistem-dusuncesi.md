# Ders 4-1: Sistem Düşüncesi

İki kişi aynı Claude Code sürümünü kullanıyor.

Biri 2 katı verimli çalışıyor. Diğeri 10 katı.

Fark modelde değil. Fark kurduğu sistemde.

---

DÜŞÜN: Bir şirkette fark yaratan şey iyi çalışanlar mı, iyi sistemler mi? Ne düşünüyorsun?

CEVAPLA: [Görüşünü paylaşır]

---

İkisi de önemli. Ama kötü bir sistemde en iyi çalışan bile verimsiz çalışır.

Claude Code da böyle. Güçlü model ama onu çevreleyen sistemi sen tasarlıyorsun.

---

## Bilgisayar Analojisi

Bir bilgisayarın parçalarıyla karşılaştır:

| Bilgisayar | Claude Code | Ne Yapar |
|-----------|-------------|---------|
| CPU | Claude modeli | Düşünme ve işleme gücü |
| RAM | Bağlam penceresi (context) | Aynı anda tutabildiği bilgi |
| Sabit Disk | Dosya sistemi | Kalıcı depolama |
| **İşletim Sistemi** | **Agent Harness** | **Her şeyi bir arada tutar** |
| Uygulamalar | Skills | Özel görevler için araçlar |

**İşletim sistemi olmadan CPU hızlı olsa da kullanılamazdı.**

Aynı şekilde: iyi model + kötü sistem = kötü sonuç.

---

## Agent Harness Nedir?

Agent Harness = Claude Code'un etrafındaki çerçeve.

Şunları yönetir:

```
┌─────────────────────────────────────┐
│           AGENT HARNESS             │
│                                     │
│  ┌──────────┐    ┌───────────────┐  │
│  │  Araçlar │    │  Güvenlik     │  │
│  │ (tools)  │    │  Sınırları    │  │
│  └──────────┘    └───────────────┘  │
│                                     │
│  ┌──────────┐    ┌───────────────┐  │
│  │  Hafıza  │    │  Bağlantılar  │  │
│  │ Sistemi  │    │  (MCP)        │  │
│  └──────────┘    └───────────────┘  │
│                                     │
│  ┌──────────────────────────────┐   │
│  │      Skills Kütüphanesi      │   │
│  └──────────────────────────────┘   │
└─────────────────────────────────────┘
```

Sen bu çerçeveyi tasarlıyorsun.

---

DÜŞÜN: Bu şemada seni en çok düşündüren kutu hangisi? Neden?

CEVAPLA: [Bir kutu seçer]

---

## Sistem Tasarımının 3 Sorusu

İyi bir Agent Harness kurmak için 3 soruyu yanıtlaman gerekiyor:

**1. Erişim:** Claude hangi sistemlere, dosyalara, bağlantılara erişebilmeli?
- Hangi klasörler?
- Hangi araçlar? (tarayıcı, email, takvim?)
- Hangi dış sistemler? (Google, Notion, Slack?)

**2. Onay:** Hangi işlemler otomatik, hangilerinde sen onay veriyorsun?
- Otomatik: tekrar eden, güvenilir işler
- Onay gerektiren: dosya silme, email gönderme, önemli değişiklikler

**3. Takip:** Kararlar ve değişiklikler nasıl kaydediliyor?
- CLAUDE.md'de mi?
- Ayrı bir log dosyasında mı?
- Git geçmişinde mi?

---

DÜŞÜN: Bu 3 soruyu kendi iş alanın için düşün. Cevapların ne olurdu?

CEVAPLA: [3 soruya cevap verir]

---

Bu cevaplar senin kişisel Agent Harness tasarımın. Bir sonraki derste bunu somutlaştıracağız.

---

## "Model Değil, Sistem Fark Yaratır"

Önemli bir hatırlatma:

Yeni bir Claude modeli çıktığında herkes heyecanlanır. "Daha akıllı!" denir.

Ama iyi sistem kurmuş biri eski modelle, kötü sistem kurmuş birinin yeni modelden daha iyi sonuç aldığı çok görüldü.

Sistem bir kez kurulur. Model zaten güncellenir.

---

**Öğrendiklerin:**
- Agent Harness = Claude Code'u çevreleyen sistem tasarımı
- Araçlar + Güvenlik + Hafıza + Bağlantılar + Skills
- 3 soru: Erişim / Onay / Takip
- Model değil, sistem fark yaratır

**Sırada ne var:** Kendi iş akışını tasarlamak — kişisel skill kütüphanesi ve "ikinci beyin" klasörü.

**Devam etmek için:** "ders 4-2" yaz
