# Taşdelen Kurban web sitesi — Claude çalışma notları

tasdelenkurban.com tanıtım sitesi. Statik site; derleme adımı yok.

## Yapı
- `dist/` — sitenin tamamı: `index.html`, `adak.html`, `iletisim.html`, `app.js`, görseller.

## Komutlar
- Yerel önizleme: `npx serve dist` → tarayıcıda gösterilen adres

## Yayın
- `main` dalında `dist/` değişince `.github/workflows/deploy.yml` değişen dosyaları SFTP ile sunucuya gönderir ve Cloudflare önbelleğini temizler. Değişiklikleri dal + PR ile yap.

## Kurallar
- Repo herkese açıktır (public): gizli bilgi, anahtar veya müşteri verisi ekleme.
- Görselleri eklerken boyutlarını küçült; sayfa hızı önemli.
- Site metinleri Türkçe.
