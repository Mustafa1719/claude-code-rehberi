# Ders 3-2: Ajanlar — Paralel Çalışma

50 müşteri mailini analiz etmen gerekiyor.

Birer birer açar, birer birer okursun. 3 saat gider.

Ya da tek bir komutla hepsini aynı anda analiz ettirirsin. 15 dakika.

Ajanlar bu farkı yaratıyor.

---

DÜŞÜN: Şimdiye kadar Claude'a çok sayıda benzer dosyayı tek tek işlettin mi? Ne kadar sürdü?

CEVAPLA: [Deneyimini paylaşır]

---

## Ajan Nedir?

Claude Code bir görevi sana verirken birden fazla "yardımcı" başlatabilir. Her yardımcı aynı anda farklı bir parçayı işler.

Bu yardımcılara **ajan** denir.

Mutfak metaforu:

```
Sen          =  Restoran sahibi (ne istediğine karar veriyorsun)
Claude       =  Şef aşçı (görevleri dağıtıyor, koordine ediyor)
Ajanlar      =  Komi aşçılar (aynı anda farklı şeyler pişiriyor)
Skills       =  Tarifler (her kominin masasında, hepsi kullanıyor)
```

Şef tek başına 10 yemeği aynı anda yapamazdı. Ama komilerle birlikte yapabilir.

---

## Hız Karşılaştırması

| Görev | Sıralı (birer birer) | Paralel (ajanlarla) |
|-------|---------------------|---------------------|
| 20 müşteri maili analiz | ~60 dakika | ~6 dakika |
| 5 farklı konu araştır | ~50 dakika | ~5 dakika |
| 30 dosyayı sınıflandır | ~90 dakika | ~10 dakika |

---

DÜŞÜN: Bu tabloya bakınca aklına hangi iş geliyor? Hangi toplu işi hızlandırmak isterdin?

CEVAPLA: [Bir iş tanımlar]

---

## Ajanları Ne Zaman Kullanırsın?

| KULLAN | KULLANMA |
|--------|---------|
| Çok sayıda benzer dosya | Tek bir dosya |
| Paralel araştırma | Sıralı işler (A bitmeden B başlayamaz) |
| Toplu üretim | Hızlı biten basit görevler |
| Birbirinden bağımsız görevler | Birbirine bağlı adımlar |

---

## Ajan Nasıl Başlatılır?

Özel bir komut yok. Sadece paralel çalışmasını söyle:

```
@musteriler/ klasöründeki tüm .txt dosyalarını paralel olarak analiz et.
Her birinden şikayetleri çıkar. Sonunda birleştir.
```

veya

```
Bu 5 konuyu aynı anda araştır:
1. [konu 1]
2. [konu 2]
3. [konu 3]
...
Hepsini ayrı bölümler halinde raporla.
```

Claude koordinatör ajan olarak devreye girer, alt ajanları başlatır, sonuçları birleştirir.

---

## Alt Ajanlar — Danışman Ekibi

İleri bir kullanım: her ajan farklı bir uzmanlık rolü ve **karakter** üstlenir.

Örnek: Yeni bir ürün lansmanı için değerlendirme istiyorsun.

```
Sen: "Bu lansman planını 3 farklı gözden değerlendir"
    ↓
├── 📊 CFO (ಠ_ಠ)  — "Veriler ne diyor? ROI nerede?"
├── 🎨 Tasarımcı (◠‿◠) — "Müşteri deneyimi nasıl? Bağ kuruldu mu?"
└── 🧑 Müşteri (•‿•) — "Ben bu ürünü neden alırım? Bana ne hissettiriyor?"
```

Her ajan kendi dilinde yanıt verir. Ana ajan sentezler:

> **CFO:** Engagement düşük. Ama ölçülebilir bir çözüm lazım.
>
> **Tasarımcı:** Kampanya ruhu yok. Duygusal bağlantı kurulmuyor.
>
> **Müşteri:** "Bu bana göre mi?" sorusunu soruyor ama cevap bulamıyor.
>
> **Sentez:** → Kişiselleştirilmiş deneyim ekle. Kullanıcı "bu benim için yapılmış" hissini bulsun.

3 farklı bakış açısı → 1 net karar. Toplantı yok, saat kaybı yok.

---

DÜŞÜN: "Danışman ekibi" modeli sana ne için kullanışlı olurdu?

CEVAPLA: [Bir senaryo önerir]

---

## Dikkat: Ajanlar Token Harcar

Her ajan ayrı bir Claude oturumudur. Paralel çalışmak = daha hızlı ama daha fazla API kullanımı.

Bu yüzden:
- Küçük dosyalar için ajanlar gerekmez
- Büyük, tekrar eden işler için idealdir
- Şüphe duyduğunda önce `/plan` ile planı gör

---

**Öğrendiklerin:**
- Ajanlar paralel çalışan yardımcı Claude oturumlarıdır
- Toplu işlerde 10 kat hız kazandırır
- Özel komut yok — "paralel çalış" veya "aynı anda" demek yeterli
- Birbirinden bağımsız görevler için idealdir

**Sırada ne var:** Plan Modu — büyük bir işe başlamadan önce planı görmek.

**Devam etmek için:** "ders 3-3" yaz
