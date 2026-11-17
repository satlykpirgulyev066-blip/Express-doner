# Express Doner — sipariş ve restoran asistanı (v2)

## İçerik

- `index.html`: Rusça/Türkçe mobil uyumlu menü, sepet, WhatsApp sipariş taslağı ve restoran SSS botu.
- `widget.js`: mevcut restoran web sitenizde sağ altta görünen sohbet balonu.
- `menu.json`: botta şu anda doğrulanabilen yemeklerin listesi. Tam site menüsü elde edildiğinde bu dosya genişletilerek hepsi bota eklenebilir.
- `siteye-ekle.html`: ana sitenin HTML koduna eklenebilecek kısa entegrasyon örneği.

## GitHub Pages üzerinde güncelleme

`https://github.com/satlykpirgulyev066-blip/Express-doner` deposunun `main` dalında `index.html`, `widget.js`, `menu.json` dosyalarını yükleyin. Mevcut `index.html` dosyasını yenisiyle değiştirin. GitHub Pages açık ise birkaç dakika sonra `https://satlykpirgulyev066-blip.github.io/Express-doner/` adresi yeni sürümü gösterir.

## Ana sitenin sağ altına baloncuk ekleme

Ana sitenin HTML'sinde `</body>` etiketinden önce şu satırı ekleyin:

```html
<script src="https://satlykpirgulyev066-blip.github.io/Express-doner/widget.js" defer></script>
```

Bunu ana sitenin düzenleyicisinde yerleştirmek gerekir. Sadece GitHub dosyalarını yüklemek mevcut `chatgpt.site` sitenizi otomatik değiştirmez. Site editörü özel JavaScript'e izin vermiyorsa başka bir entegrasyon yöntemi gerekecektir.

## Bot ne bilir?

Çalışma saatleri (rehberler: 10:00–21:00 her gün; teyitli değil), adres, telefon, teslimat hakkında belirsiz koşullar, menüde doğrulanmış yemekler ve sipariş sepeti. Teslimat koşulları ve sipariş kabulü hakkında tahminde bulunmaz. WhatsApp'a hazırlanan mesajı göndermek ziyaretçinin işlemiyle gerçekleşir.

## Fiyatlar

Şu anda yalnızca daha önce sağlanan, doğrulanabilen isimler/fiyatlar kullanılıyor. Ana siteye bu ortamdan erişim sağlanamadığı için sitedeki tüm 85+ menü ürünü otomatik aktarılamadı. `menu.json`'u gerçek menü verileriyle değiştirince bot bütün ürünleri gösterebilir. Fiyatı gram üzerinden belirlenen Tomahawk ürününü ağırlık doğrulanmadan sepete eklemiyoruz.
