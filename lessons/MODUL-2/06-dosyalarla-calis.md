# Ders 2-1: Dosyalarla Çalışmak

Birinin sana 20 klasör dolusu dosya verdiğini hayal et. "Bunları analiz et" dedi ve gitti.

ChatGPT'ye açamazsın. Email'e yapıştıramazsın.

Claude Code'da tek bir sembolle hepsini işaret edebilirsin: **@**

---

DÜŞÜN: Şu ana kadar dosyalarla çalışırken en çok neyi zaman alıyordu? (Aramak? Kopyalamak? Özetlemek?)

CEVAPLA: [Deneyimini paylaşır]

---

## @ Sembolü Nedir?

`@` = "şu dosyaya / klasöre bak" demek.

Kullanım:

```
@dosya_adi.txt    → tek dosyayı referans al
@klasor_adi/      → tüm klasörü referans al
```

Örnek komutlar:

```
@toplanti_notu.txt dosyasındaki görevleri listele
@musteriler/ klasöründeki tüm maiileri özetle
@rapor.pdf içindeki sayıları bir tabloya dök
```

---

## 5 Temel Desen

Dosyalarla çalışmanın 5 temel yolu:

| # | Desen | Ne Yapar | Örnek |
|---|-------|---------|-------|
| 1 | **Tek Dosya → Çıkar** | Bir dosyadan bilgi çek | `@toplanti.txt görevleri listele` |
| 2 | **Klasör → Sentezle** | Birçok dosyayı tek bakışta analiz et | `@musteriler/ ortak şikayetleri bul` |
| 3 | **Şablon Uygula** | Dosya + format = tutarlı çıktı | `@veri.xlsx haftalık rapor şablonuna dök` |
| 4 | **Görsel → Analiz** | Ekran görüntüsü yapıştır | `Ctrl+V → "Bu görseldeki metni çıkar"` |
| 5 | **Web → Araştır** | İnternetten bilgi topla | `"Claude Code için en iyi kaynakları bul"` |

---

DÜŞÜN: Bu 5 desenden hangisi senin için en kullanışlı? Hangi iş için kullanırdın?

CEVAPLA: [Bir desen seçer]

---

İZLE: `scenarios/dosya-kaos/` klasörünün içeriğini listele ve kullanıcıya göster.

---

Şimdi sıra sende.

DÜŞÜN: `@scenarios/dosya-kaos/` yazarak bu klasördeki dosyaları organize etmemi söyle. Bir cümleyle — nasıl organize edilmesini istiyorsun?

CEVAPLA: [Komutunu yazar]

---

İZLE: Kullanıcının komutunu uygula. dosya-kaos klasörünü mantıklı alt klasörlere ayır, dosya isimlerini temizle, bir özet listesi oluştur.

---

DÜŞÜN: Sonucu gördün mü? Beklediğin gibi miydi?

CEVAPLA: [Yorumunu paylaşır]

---

## Pratik İpuçları

**Büyük dosyalarda:** Claude'un bir "bağlam penceresi" (context window) var — yani bir seferde okuyabileceği maksimum metin miktarı. Çok büyük dosyalarda `/compact` komutuyla sıkıştır.

**Çok sayıda dosyada:** Önce `/plan` ile planla — 50 dosyayı tek hamlede işlemeden önce planı gör.

**Görsel dosyalarda:** PDF ve resim dosyalarını doğrudan Claude Code'a sürükle-bırak ya da terminale dosya yolunu yaz.

---

**Öğrendiklerin:**
- `@` sembolü dosya ve klasörleri referans almanın yolu
- 5 temel desen: Çıkar / Sentezle / Şablon / Görsel / Web
- Büyük veri setlerinde `/plan` ve `/compact` yardımcı olur

**Sırada ne var:** Komutlar — en önemli 8 slash komutu ve 3 çalışma modu.

**Devam etmek için:** "ders 2-2" yaz
