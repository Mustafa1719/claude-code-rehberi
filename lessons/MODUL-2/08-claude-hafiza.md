# Ders 2-3: CLAUDE.md — Projenin Hafızası

Her yeni Claude Code oturumu boş bir kağıtla başlar.

Adını bilmez. Ne üzerinde çalıştığını bilmez. Nasıl davranmasını istediğini bilmez.

Her seferinde yeniden tanışmak zorunda mısın?

Hayır. Bunun için CLAUDE.md var.

---

DÜŞÜN: Yeni işe giren birine her sabah aynı şeyleri anlatmak zorunda kalsaydın ne yapardın?

CEVAPLA: [Bir not, brifing belgesi, el kitabı gibi bir şey söyler]

---

Tam. CLAUDE.md de tam olarak bu.

Her oturum başladığında Claude otomatik olarak CLAUDE.md dosyasını okur. Kimin olduğunu, ne üzerinde çalıştığını, nasıl davranması gerektiğini öğrenir.

Sabah masasına koyduğun brifing belgesi.

---

## Anayasa Metaforu

```
CLAUDE.md  =  Anayasa
               (kalıcı, en yüksek otorite)
                      ↓
Promptlar  =  Günlük kararlar
               (anayasaya uymak zorunda)
```

Örnek: CLAUDE.md'ye "Türkçe cevap ver" yazdıysan, bir promptta "answer in English" desen bile — Claude Türkçe cevap verir.

CLAUDE.md her şeyin üzerinde.

---

## CLAUDE.md Hiyerarşisi

Birden fazla CLAUDE.md olabilir:

```
~/.claude/CLAUDE.md          ← Tüm projeler için geçerli (genel kurallar)
     ↓
proje_klasoru/CLAUDE.md      ← Bu proje için geçerli (özel kurallar)
     ↓
alt_klasor/CLAUDE.md         ← Bu alt klasör için geçerli (çok nadir)
```

Çoğu zaman sadece proje klasöründeki yeterli.

---

DÜŞÜN: Sana her gün yardım eden bir asistan olsaydı, ona ne bilmesini isterdin? 3 şey say.

CEVAPLA: [3 şey listeler]

---

İşte CLAUDE.md'ye tam olarak bunları yazacaksın.

---

## İlk CLAUDE.md'yi Oluştur

Terminale şunu yaz:

```
/init
```

Claude projeyi analiz eder ve otomatik bir CLAUDE.md taslağı oluşturur.

İZLE: `/init` komutunu çalıştır, oluşturulan CLAUDE.md dosyasını göster.

---

DÜŞÜN: Oluşturulan CLAUDE.md'ye bak. Seni şaşırtan bir şey var mı? Eksik gördüğün bir şey var mı?

CEVAPLA: [Gözlemini paylaşır]

---

## İyi CLAUDE.md Nasıl Olur?

3 kural — basit tut:

**1. En önemli kurallar en üste**
Claude dosyayı yukarıdan okur. Kritik şeyleri başa yaz.

**2. Madde işareti + kısa başlık formatı**

```markdown
## Genel Kurallar
- Türkçe cevap ver
- Her değişiklikten önce sor
- Kısa ve net ol — uzun açıklama yapma
```

**3. "Her zaman" ve "Asla" gibi net ifadeler kullan**

```markdown
- Her zaman değişiklik yapmadan önce planı göster
- Asla .env dosyasını düzenleme
- Asla commit yapma, ben sorana kadar
```

---

## Şimdi Kendininkini Yaz

İZLE: `scenarios/hafiza-kur/` klasörünü aç. İçinde yönlendirici sorular var. Onları okuyarak kendi CLAUDE.md'ni birlikte yazalım.

---

DÜŞÜN: Sorulara cevap verdikten sonra oluşan CLAUDE.md'yi oku. Bu seni tanımlıyor mu?

CEVAPLA: [Değerlendirmesini paylaşır]

---

**Öğrendiklerin:**
- Her oturum boş başlar — CLAUDE.md kalıcı hafıza sağlar
- CLAUDE.md bir anayasadır — tüm promptların üzerindedir
- `/init` ile otomatik oluşturulur, sonra özelleştirilir

**Sırada ne var:** Modül 3 — Skills, Ajanlar, Plan Modu. Tekrar eden işleri otomatikleştirme zamanı.

**Devam etmek için:** "modül 3" veya "ders 3-1" yaz
