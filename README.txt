EXPRESS DONER — SİPARİŞ BOTU (İLK SÜRÜM)
=======================================

DOSYALAR
- index.html : Telefon ve bilgisayarda açılan sipariş botu.

NASIL DENENİR?
1. index.html dosyasını telefona veya bilgisayara kaydedin.
2. Tarayıcıda açın.
3. Menüden ürün ekleyin ve sepeti açın.
4. Ad / telefon girerek sipariş taslağını oluşturun.
5. 'Kopyala' ya da 'Paylaş' ile mesajı restoran yetkilisine iletin.

ÖNEMLİ
Bu ilk sürüm bir DEMO'dur. Siparişler sunucuya kaydedilmez,
restorana otomatik ulaşmaz ve ödeme alınmaz.
Müşteri bilgileri sunucuya gönderilmez. Sepetteki ürünler cihazda saklanır.

RUSÇA / TÜRKÇE
Sağ üstte RU / TR düğmesi bulunur. Müşteri arayüzü Rusça açılır.

GITHUB PAGES İLE YAYINLAMA
1. GitHub'da yeni bir public repository açın (örn: express-doner-bot).
2. index.html dosyasını bu repository'nin köküne yükleyin.
3. Settings > Pages > Build and deployment > Deploy from a branch seçin.
4. Branch: main / (root) seçip Save'e basın.
5. Pages'in verdiği web adresini açın.

RESTORAN WHATSAPP NUMARASI EKLEME
index.html içinde şu satırı bulun:
  const CONFIG = { whatsappPhone: "" };
Restoranın doğrulanmış numarasını ülke koduyla yalnızca rakam olarak girin:
  const CONFIG = { whatsappPhone: "79XXXXXXXXX" };
Bu durumda 'Paylaş' yerine 'WhatsApp' görünür ve sipariş metni
belirtilen numarayla sohbet açılarak gönderilmeye hazır hale gelir.
Mesaj ancak müşteri WhatsApp'ta gönderme işlemini tamamlarsa iletilir.

MENÜYÜ DÜZENLEME
index.html içindeki PRODUCTS listesinden ürün adını ve fiyatları değiştirin.
Şu an 8 adet geçmişte onaylanan fiyat kullanıldı. Yeni ürünleri ve
fiyatları işletme onayladıktan sonra ekleyin.

CANLI SÜRÜM İÇİN SONRAKİ ADIMLAR
- Gerçek Express Doner logosu ve yemek fotoğrafları
- Restoranın WhatsApp numarası / sipariş alma kanalı
- Sipariş veritabanı + yönetim paneli + gerçek bildirimler
- Çalışma saatleri, teslimat / gel-al kuralları, ödeme entegrasyonu
