# Ders 3-3: Plan Modu — Önce Düşün

Büyük bir işi doğrudan başlatmak cazip gelir.

Ama Claude'un planlamadan başlaması bazen şaşırttığı şeyler yapmasına yol açar. Dosyaları yanlış yere koyar. Yanlış formatta çıktı üretir. Sonra geri almak gerekir.

Plan Modu bunu önler.

---

DÜŞÜN: Büyük bir projeye başlamadan önce plan yapar mısın? Neden yapar ya da yapmaz mısın?

CEVAPLA: [Alışkanlığını paylaşır]

---

## Plan Modu Ne Yapar?

Plan Modunda Claude:

- Dosyaları **okur** ama **dokunmaz**
- Bir plan üretir
- Sen planı onaylarsın
- Sonra çalışır

```
Normal Mod:   Söyle → Hemen Yap
Plan Modu:    Söyle → Planla → Sen Onayla → Yap
```

---

## Neden Önemli?

İki senaryo:

**Senaryo A — Plan Modu olmadan:**
```
> 200 dosyalı bu klasörü yeniden organize et
Claude: [Hemen başlar. 30 dakika sonra...]
Claude: Tamamlandı.
Sen: Ama ben bu formatta istemiyordum...
```

**Senaryo B — Plan Modu ile:**
```
> 200 dosyalı bu klasörü yeniden organize et
Claude: [Dosyaları okur, düşünür]
Claude: "Plan: 5 ana klasör oluşturacağım. Şunları yapacağım..."
Sen: Mükemmel / Dur, şunu değiştir
Claude: Onaylandı. Başlıyorum.
```

Planlama için harcanan 5 dakika, yeniden yapmak için harcanan 50 dakikayı önler.

---

## Plan Moduna Nasıl Girilir?

**Klavye kısayolu:**

```
Shift + Tab  →  Plan Moduna geç (veya Auto-Accept'ten geç)
Esc          →  Geri dön
```

Terminalde mod göstergesi değişir:
```
[PLAN]  >           ← Plan modunda
>                   ← Normal modda
```

**Alternatif — komutla:**

```
/plan
```

Bu komutu yazdıktan sonra görevini anlat.

---

DÜŞÜN: `Shift + Tab` kombinasyonunu dene. Mod göstergesi değişti mi?

CEVAPLA: [Gördüğünü anlatır]

---

## Plan Modunu Kullan

İZLE: Plan Moduna geç. Şu görevi ver:

```
@scenarios/dosya-kaos/ klasörünü temizlemek istiyorum. Nasıl bir yapı oluşturmayı planlarsın?
```

Claude dosyaları okuyacak, bir plan üretecek. Sen planı onaylamadan hiçbir şey değişmeyecek.

---

DÜŞÜN: Plan geldi mi? Planı okudum — mantıklı mı? Değiştirmek istediğin bir şey var mı?

CEVAPLA: [Planı değerlendirir]

---

İstediğini söyle. Claude planı revize eder. Onayladıktan sonra çalıştır.

---

## Plan Modu İçin En İyi Durumlar

```
✅ Birçok dosyayı etkileyen işler
✅ Geri alması zor değişiklikler
✅ Yeni bir işi ilk kez yapıyorsan
✅ Büyük klasör organizasyonları
✅ Toplu yeniden adlandırma işlemleri

❌ Basit, tek dosya işlemleri
❌ Hızlı test ve deneme
❌ Zaten çok iyi bildiğin tekrar eden işler
```

---

**Öğrendiklerin:**
- Plan Modu: okur ama dokunmaz — planı onayladıktan sonra çalışır
- `Shift + Tab` veya `/plan` ile girilir
- Büyük ve geri dönülmesi zor işler için ideal
- "Planla, onayla, çalıştır" döngüsü hataları önler

**Sırada ne var:** Modül 4 — büyük resim. Claude Code'u bir kişisel işletim sistemi olarak kurmak.

**Devam etmek için:** "modül 4" veya "ders 4-1" yaz
