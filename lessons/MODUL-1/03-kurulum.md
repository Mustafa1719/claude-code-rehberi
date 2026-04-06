# Ders 1-1: Kurulum

> **Bu siteye Claude Code üzerinden ulaştıysan kurulum ve indirme adımlarını zaten tamamladın.**
> Doğrudan ilk göreve geçebilirsin → **"ders 1-3" yaz**

---

Terminal kelimesini duyunca "bu benim için değil" diye düşündüysen — dur.

Bu derste terminal nedir bilmeden Claude Code kuracaksın.

---

DÜŞÜN: Hangi işletim sistemini kullanıyorsun?

- **Mac** (Apple logosu olan bilgisayar)
- **Windows** (Microsoft, mavi ekran :)
- **Linux** (genellikle programcılar kullanır)

CEVAPLA: Mac / Windows / Linux

---

## Terminal Nedir?

Terminal = bilgisayarına yazarak komut verdiğin siyah (veya beyaz) ekran.

Mouse yerine klavye kullanırsın. Görsel bir arayüz yoktur. Ama çok güçlüdür.

Nasıl açılır:

| İşletim Sistemi | Nasıl Açılır |
|----------------|-------------|
| **Mac** | `Cmd + Boşluk` → "terminal" yaz → Enter |
| **Windows** | Başlat menüsü → "PowerShell" yaz → Enter |
| **Linux** | `Ctrl + Alt + T` |

Açtığında şöyle bir şey göreceksin:

```
kullaniciadi@bilgisayar ~ %
```

veya

```
PS C:\Users\kullaniciadi>
```

Bu normal. Bilgisayar senden komut bekliyor.

---

DÜŞÜN: Terminali açtın mı? Ekranda ne görüyorsun?

CEVAPLA: [Ne gördüğünü anlatır]

---

## Kurulum Komutu

Şimdi aşağıdaki komutu terminale yaz ve Enter'a bas:

**Mac / Linux / WSL için:**
```
curl -fsSL https://claude.ai/install.sh | bash
```

**Windows (PowerShell) için:**
```
irm https://claude.ai/install.ps1 | iex
```

> **Not:** Windows'ta kurulum için [Git for Windows](https://git-scm.com/downloads/win) yüklü olmalı.

Kurulum 1-3 dakika sürebilir. Yüzlerce satır metin kayacak — normal.

---

DÜŞÜN: Kurulum tamamlandı mı? Son satırda ne yazıyor?

CEVAPLA: [Son satırı kopyalar ya da anlatır]

---

## Sorun Giderme

Hata aldıysan — panik yapma. Yaygın sorunlar:

| Hata Mesajı | Anlam | Çözüm |
|------------|-------|-------|
| `command not found: curl` | curl yüklü değil | Mac: `brew install curl` / Windows: PowerShell yöntemini dene |
| `permission denied` | Yetki sorunu | `sudo bash` ile tekrar dene (Mac/Linux) |
| `network error` | İnternet sorunu | Bağlantını kontrol et |
| Windows'ta hata | Git yüklü değil | [git-scm.com](https://git-scm.com/downloads/win)'den kur, terminali yeniden aç |

Başka bir hata gördüysen — tam mesajı buraya yaz, birlikte çözeriz.

---

## Kurulumu Doğrula

Terminal'e şunu yaz:

```
claude --version
```

Şuna benzer bir şey görmelisin:

```
claude 1.x.x
```

---

DÜŞÜN: `claude --version` yazdın mı? Ne gördün?

CEVAPLA: Versiyon numarası / Hata mesajı

---

## Giriş Yap

Şimdi terminale şunu yaz:

```
claude
```

İlk çalıştırmada Anthropic hesabına giriş yapman isteniyor. Tarayıcı açılacak — giriş yap, geri dön.

> **Önemli:** Claude Code, **Claude Pro veya Max aboneliği** gerektirir. Ücretsiz hesapla çalışmaz. Abonelik için claude.ai adresini ziyaret et.

Giriş tamamlandığında terminalde şunu göreceksin:

```
>
```

Bu, Claude Code'un seni beklediği anlamına geliyor.

---

DÜŞÜN: Terminalde `>` işaretini gördün mü?

CEVAPLA: Evet / Hayır

---

**Öğrendiklerin:**
- Terminal siyah ekran değil, güçlü bir komut arayüzü
- npm ile Claude Code kuruldu
- `claude` komutuyla oturum açıldı

**Sırada ne var:** İlk gerçek görevi veriyorsun — ve "sormak" ile "yaptırmak" farkını bizzat hissediyorsun.

**Devam etmek için:** "ders 1-2" yaz
