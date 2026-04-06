# Ders 1-2: İlk Oturum

Kurulum tamam. Şimdi Claude Code'u başlatma vakti.

Terminalde şunu yaz ve Enter'a bas:

```
claude
```

Birkaç saniye içinde ekranda `>` işareti görünecek — bu Claude Code'un seni beklediğini gösterir.

---

DÜŞÜN: Şu an terminalde `>` işaretini görüyor musun?

CEVAPLA: Evet / Hayır

> Göremiyorsan: `claude` komutunu yazdın mı? Yazdıysan ve hâlâ göremiyorsan — tam olarak ne görüyorsun, yazar mısın?

---

## Senaryo: Dağınık Dosyalar

Şu an `scenarios/ilk-gorev/` klasöründe 8 dosya var. Hepsi karmaşık isimli, tarihsiz, düzensiz.

İZLE: `scenarios/ilk-gorev/` klasörünün içeriğini listele ve kullanıcıya göster.

```
toplanti_notlari_son_FINAL_v3.txt
rapor - kopya.docx
Rapor_2024_TASLAK.docx
musteri_gorusme_notlari.txt
sunum_GUNCEL.pptx
sunum_yedek_eski.pptx
analiz_excel_son.xlsx
TODO_listesi_BAKILACAK.txt
```

---

DÜŞÜN: Bu klasörü görüyorsun. Şimdi bana şunu söyle: ChatGPT'ye nasıl sorardın bu sorunu?

CEVAPLA: ["Bu dosyaları nasıl organize etmeliyim?" gibi bir şey]

---

Dikkat et. "Nasıl organize etmeliyim?" diye sorsan ne alırsın?

Bir liste alırsın. Tavsiyeler alırsın. Belki bir tablo alırsın.

Ama dosyalar hâlâ yerinde durur.

---

## Sormak vs Yaptırmak

| ❌ ChatGPT Modu (Sormak) | ✅ Claude Code Modu (Yaptırmak) |
|--------------------------|--------------------------------|
| "Bu dosyaları nasıl düzenlemeliyim?" | "Bu dosyaları düzenle." |
| "Hangi klasör yapısını önerir misin?" | "Mantıklı bir klasör yapısı kur." |
| "Bu raporu nasıl özetlemeliyim?" | "Bu raporu özetle." |
| Tavsiye alırsın | Sonuç alırsın |

Fark tek kelime: **nasıl** vs **yap**.

---

DÜŞÜN: Şimdi senden istiyorum: Bu 8 dosyayı organize etmemi söyle. Tek bir cümleyle, sanki bana iş veriyorsun.

CEVAPLA: [Bir komut yazar — "Bu dosyaları organize et" gibi]

---

İZLE: Kullanıcının verdiği komutu uygula. `scenarios/ilk-gorev/` klasörünü şu yapıya göre düzenle:

```
scenarios/ilk-gorev/
├── raporlar/
│   ├── Rapor_2024_TASLAK.docx
│   └── rapor_kopya.docx
├── sunumlar/
│   ├── sunum_GUNCEL.pptx
│   └── sunum_yedek_eski.pptx
├── notlar/
│   ├── toplanti_notlari.txt
│   └── musteri_gorusme_notlari.txt
├── analizler/
│   └── analiz_excel.xlsx
└── gorevler/
    └── TODO_listesi.txt
```

Dosyalar taşındı. İsimlerdeki gereksiz ekler (`_son`, `_FINAL`, `_GUNCEL` vb.) temizlendi.

---

DÜŞÜN: Klasöre bak. Dosyalar taşındı mı? Nasıl hissettirdi?

CEVAPLA: [Deneyimini paylaşır]

---

İşte bu. Sen bir cümle yazdın. Ben planladım, klasörler oluşturdum, dosyaları taşıdım, isimleri düzelttim.

Seçim:
- ❌ "Nasıl organize etmeliyim?" → tavsiye
- ✅ "Organize et." → iş bitti

---

## Delegasyon Formülü

Bundan sonra her komut verirken şunu hatırla:

```
NE istiyorum  +  NASIL bir sonuç bekliyorum
```

Örnek:
- "Bu toplantı notlarını görev listesine dönüştür. Her görevin yanına sorumlu kişiyi yaz."
- "Bu 10 dosyayı incele ve hangilerinin güncellenmesi gerektiğini söyle."
- "Bu klasörü organize et. Tarihsiz dosyalara bugünün tarihini ekle."

NE + NASIL = Net görev.

---

**Öğrendiklerin:**
- "Nasıl yapmalıyım?" sormak = tavsiye almak
- "Yap." demek = iş bitmek
- Delegasyon formülü: NE istiyorum + NASIL bir sonuç

**Sırada ne var:** Claude Code'u kullanırken dosyaları da görmek — çift panel kuruyoruz.

**Devam etmek için:** "ders 1-3" yaz
