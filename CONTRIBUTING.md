# 🤝 Katkıda Bulunma Rehberi

Bu repoya katkıda bulunmak istediğin için teşekkürler! Her katkı, ne kadar küçük olursa olsun, bu kaynağı topluluk için daha iyi hale getirir.

---

## 📋 İçindekiler

- [Nasıl Katkıda Bulunabilirim?](#nasıl-katkıda-bulunabilirim)
- [Yeni Araç Eklemek](#yeni-araç-eklemek)
- [Yeni Proje Eklemek](#yeni-proje-eklemek)
- [Mevcut Araç Güncellemek](#mevcut-araç-güncellemek)
- [Hata veya Sorun Bildirmek](#hata-veya-sorun-bildirmek)
- [PR Süreci](#pr-süreci)
- [Kalite Standartları](#kalite-standartları)
- [Davranış Kuralları](#davranış-kuralları)

---

## Nasıl Katkıda Bulunabilirim?

Katkı türleri ve zorluk seviyeleri:

| Katkı Türü | Zorluk | Label |
| --- | --- | --- |
| Yeni araç ekle | ⭐ Kolay | `good first issue` |
| Yeni proje ekle | ⭐⭐ Orta | `enhancement` |
| Fiyat / link güncelle | ⭐ Kolay | `content update` |
| Türkçe destek bilgisi ekle | ⭐ Kolay | `content update` |
| Yeni kategori öner | ⭐⭐ Orta | `discussion` |
| Araç karşılaştırması yaz | ⭐⭐ Orta | `enhancement` |
| Repo yapısını geliştir | ⭐⭐⭐ Zor | `enhancement` |

---

## Yeni Araç Eklemek

### Adım 1. Reponu Fork'la

```bash
git clone https://github.com/YOUR_ORG/awesome-ai-tools.git
cd awesome-ai-tools
git checkout -b add/arac-adi
```

### Adım 2. Doğru kategoriye git

`/categories/` klasöründen uygun `.md` dosyasını aç. Hangi kategoriye gireceğinden emin değilsen Issue aç, birlikte karar verelim.

### Adım 3. Aracı şu formatta ekle

```markdown
### Araç Adı
- 🔗 **Link:** [website.com](https://website.com)
- 📝 **Açıklama:** Aracın ne işe yaradığı, 1-2 cümle.
- 💰 **Fiyatlandırma:** Ücretsiz / Freemium / Ücretli
- 🌍 **Türkçe Desteği:** Var / Yok / Kısmi
- ⭐ **Topluluk Notu:** X/5
- 🧪 **Test Eden:** @github_kullanici_adin
- 💬 **Kullanım Notu:** Gerçek deneyiminden kısa bir yorum. Ne işine yaradı? Dikkat edilmesi gereken bir şey var mı?
```

### Adım 4. PR Aç

```bash
git add .
git commit -m "feat: [Araç Adı] eklendi - [Kategori]"
git push origin add/arac-adi
```

PR başlığı: `feat: [Araç Adı] eklendi`
PR açıklaması: Aracı neden eklediğini, nasıl test ettiğini kısaca yaz.

---

## Yeni Proje Eklemek

Bu repodaki araçları kullanarak geliştirdiğiniz projeleri paylaşmak için `projects/README.md` dosyasına şu formatta ekleme yapın:

```markdown
### [Proje Adı]
- 📝 **Özet:** Projenin ne yaptığı ve hangi sorunu çözdüğü.
- ⚙️ **Teknoloji Yığını:** (Örn: Python, Gemini API, LangChain)
- 👤 **Katkıda Bulunan:** [@github_kullanici_adi] veya [linkedin_linki]
- 🔗 **Link:** [Canlı Link](https://link.com) (Canlıya alınmış bir proje ise linki)
```

Ekleme yaptıktan sonra commit edin ve PR açın. PR başlığı `feat: [Proje Adı] projesi eklendi` olmalıdır.

---

## Mevcut Araç Güncellemek

Fiyat değişikliği, link bozukluğu veya yanlış bilgi mi fark ettin?

1. Doğrudan ilgili `.md` dosyasını düzenle
2. Commit mesajı: `fix: [Araç Adı] fiyat/link/bilgi güncellendi`
3. PR aç, kısa bir açıklama yeterli.

---

## Hata veya Sorun Bildirmek

[Issues](https://github.com/Turkish-AI-Community/awesome-ai-tools/issues) sekmesinden yeni bir issue aç ve şu şablonu kullan:

```text
**Sorun:** Nedir?
**Nerede:** Hangi kategori / araç?
**Beklenen:** Ne olmalıydı?
**Ekstra:** Varsa ekran görüntüsü veya link
```

---

## PR Süreci

1. PR açıldıktan sonra bir maintainer en geç **3 iş günü** içinde inceleme yapar
2. Değişiklik istenirse yorum olarak bildirilir
3. Onaylanan PR'lar `main` branch'e merge edilir
4. Katkın `README` istatistiklerine otomatik yansır

---

## Kalite Standartları

Katkının kabul edilmesi için:

- [ ] Araç gerçekten test edilmiş olmalı (varsayıma dayalı ekleme yok)
- [ ] Link aktif ve doğru olmalı
- [ ] Format eksiksiz doldurulmuş olmalı
- [ ] Reklam amaçlı veya spam içerik olmamalı
- [ ] Türkçe alanlar Türkçe yazılmalı
- [ ] Açıklama kısa, net ve tarafsız olmalı
- [ ] Teknik bilgiler doğrulanmış ve güncel olmalı — yanıltıcı içerik kabul edilmez
- [ ] Telif hakkıyla korunan materyaller izinsiz paylaşılmamalı
- [ ] İçerik, topluluğun Etik İlkeler Beyannamesi'ne uygun olmalı

---

## 🌟 Sık Sorulan Sorular

**Bir aracı test etmedim ama çok iyi olduğunu duydum, ekleyebilir miyim?**  
Hayır. Sadece bizzat kullandığın araçları ekle. Duyuma dayalı eklemeler kabul edilmez.

**Bir araç ücretli ama çok işlevsel. Ekleyebilir miyim?**  
Evet. Fiyatlandırma kriteri kaliteyi değil bilgiyi etkiler, sadece doğru etiketle.

**Yeni bir kategori önermek istiyorum.**  
Harika! Önce bir Issue aç, tartışalım. Onaylanırsa kategoriye ait `.md` dosyasını ekleyip PR açabilirsin.

---

## Davranış Kuralları

Bu topluluğa katkıda bulunan herkes:

- Saygılı ve yapıcı bir dil kullanır
- Farklı deneyim seviyelerindeki katkıcılara destek olur
- Ticari çıkar gütmeden, topluluk için katkıda bulunur
- Kapsayıcı ve erişilebilir bir ortam için çaba gösterir

Detaylı kurallar için [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md) dosyasına bakabilirsin.

---

### Her Katkı Önemlidir

Büyük fikirler küçük PR'larla başlar. 🚀
