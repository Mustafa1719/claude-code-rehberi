# Kaynaklar ve Bağlantılar

Bu kursun hazırlanmasında kullanılan ve öğrenmeye devam etmek için önerilen kaynaklar.

---

## Bu Kursu Hazırlarken Kullanılan Kaynaklar

| Kaynak | Tür | Konusu |
|--------|-----|--------|
| `cowork-complete-guide/` | Kurs (12 ders) | DÜŞÜN/İZLE/CEVAPLA format ilhami, delegasyon modeli |
| `ccforeveryone-kaynak.md` | Web kursu özeti | Kurulum, komutlar, ajanlar, CLAUDE.md |
| `Claude Code (Beginner → Advanced).pdf` | Newsletter | Kurulum, Skills, MCP, gerçek iş akışları |
| `Claude Code Cheat Sheet.pdf` | Referans kartı | Tüm komutlar, kısayollar, modlar |
| `𝐀𝐈 𝐅𝐥𝐮𝐞𝐧𝐜𝐲.docx` | Strateji | AI Fluency kavramı, skill gap |
| `Operating System (Harness).docx` | Strateji | Agent Harness, sistem tasarımı |
| `Claude Plugins -Claude Skills.docx` | Kavram | Simple Chat → Skills → Plugins skalası |
| `Anatomy of the _claude folder.jpg` | Görsel | .claude klasörü yapısı |

---

## Öğrenmeye Devam Etmek İçin

### Genel Claude Code

| Kaynak | İçerik |
|--------|--------|
| **ccforeveryone.com** | Kapsamlı Claude Code rehberi — kurulum, dosyalar, komutlar, ajanlar |
| **claude.ai/docs** | Resmi Anthropic dökümantasyonu |
| **anthropic.com/claude-code** | Resmi Claude Code sayfası |

### Topluluk

| Platform | Ne Bulursun |
|----------|------------|
| **X (Twitter) — #ClaudeCode** | Gerçek kullanım örnekleri, güncel haberler |
| **Reddit r/ClaudeAI** | Sorular, deneyimler |
| **Discord — Anthropic** | Canlı topluluk desteği |

---

## MCP Sunucuları (İleri Seviye)

MCP (Model Context Protocol) ile Claude'u dış sistemlere bağlayabilirsin:

| MCP | Ne Bağlar | Kurulum Paketi |
|-----|-----------|---------------|
| **Google Drive** | Drive dosyaları | `@google/drive-mcp` |
| **GitHub** | Repolar, issues, PR'lar | `@github/github-mcp-server` |
| **Notion** | Sayfalar, veritabanları | `@modelcontextprotocol/notion` |
| **Slack** | Kanallar, mesajlar | `@modelcontextprotocol/slack` |
| **n8n** | n8n workflow'ları | `@anthropic/n8n-mcp` |
| **Tarayıcı** | Web siteleri, formlar | `@playwright/mcp` |

Kurulum talimatları için: `~/.claude/settings.json` → `mcpServers` bölümü

---

## Önerilen Öğrenme Sırası

Bu kursu tamamladıktan sonra:

```
1. CLAUDE.md'ni geliştir (bu hafta)
   → Kendi çalışma stiline göre özelleştir

2. İlk 3 Skill'ini oluştur (bu ay)
   → Tekrar eden işlerini dönüştür

3. MCP'ye başla (önümüzdeki ay)
   → Google Drive veya GitHub ile başla

4. Ajan iş akışı tasarla (2. ay)
   → Bir toplu işi ajanlarla otomatikleştir

5. Custom Sub-Agents (3. ay)
   → Danışman ekibi modelini dene
```

---

## Araçlar

| Araç | Ne İçin | Nereden |
|------|---------|---------|
| **VS Code** | Görsel çalışma alanı | code.visualstudio.com |
| **Nimbalyst** | Terminal gerektirmeyen arayüz | nimbalyst.com |
| **Claude Desktop** | Masaüstü uygulaması | claude.ai/download |

---

*Bu kursun ana dosyası: `START-HERE.md`*
*Hızlı referans: `referans/cheat-sheet-ozet.md`*
