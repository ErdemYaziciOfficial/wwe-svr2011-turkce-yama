# WWE SmackDown vs. Raw 2011 — PC Türkçe Yama

Türkçe menüler, RTWM hikâye diyalogları, PC arayüzü ve Türkçe karakter desteği. Mevcut dillerin yanına **TÜRKÇE** seçeneği eklenir.

**İlk kez kuruyorsan:** önce oyunu PC'de çalıştır, sonra Türkçe yamayı kur. Aşağıda ikisi de sırasıyla anlatılıyor.

**Oyun zaten bilgisayarında açılıyorsa:** doğrudan **[2. Türkçe yamayı indir](#2-türkçe-yamayı-indir)** bölümüne geç. Bu yama PC portunun **2.0.6** sürümü için hazırlanmıştır.

## 1. Oyun bilgisayarında kurulu değilse

### Önce ne gerekiyor?

- Bir Windows bilgisayar.
- Kendi **Xbox 360 sürümü** WWE SmackDown vs. Raw 2011 oyununun `.iso` dosyası. ISO, oyun diskinin dosya hâlidir. **PS2, PS3, PSP ve Wii sürümleri bu kurulumda çalışmaz.**
- Aşağıdan indireceğin PC başlatıcısı. Başlatıcı ve Türkçe yama tek başına oyunun tamamı değildir; ISO bu indirmelerde bulunmaz.

### PC başlatıcısını indir ve oyunu kur

1. **[PC başlatıcısını indirmek için buraya tıkla — SvR2011-PC-v2.0.6.zip](https://github.com/KaikoClanworth1/wwe-svr2011-pc/releases/download/v2.0.6/SvR2011-PC-v2.0.6.zip)**.
2. İndirme bitince Windows'ta **İndirilenler** klasörünü aç. `SvR2011-PC-v2.0.6.zip` dosyasına sağ tıkla → **Tümünü Ayıkla** → **Ayıkla**. Bu işlem ZIP'in içindekileri normal bir klasöre çıkarır.
3. Çıkan klasörü aç. İçindeki **`SvR2011 Launcher.exe`** dosyasına çift tıkla. Dosya uzantıları gizliyse adı yalnızca **SvR2011 Launcher** görünebilir.
4. Başlatıcıda **Install** sekmesini aç.
5. **Your disc image** alanında kendi oyununun `.iso` dosyasını seç.
6. **Install to** alanında oyun için **boş bir klasör** seç. Örneğin `C:\Oyunlar\SvR2011`. **Bu klasörün yerini unutma; Türkçe yamayı da buraya kuracağız.**
7. **Install** düğmesine bas ve işlemin tamamlanmasını bekle.
8. **Play** sekmesine geçip **Play** düğmesine bas. Oyunun açıldığını gördükten sonra **oyunu ve başlatıcıyı kapat**.

PC portu **KaikoClanworth1 ve katkıcılarına** aittir. [Orijinal proje ve kurulum rehberi](https://github.com/KaikoClanworth1/wwe-svr2011-pc#install-and-play).

## 2. Türkçe yamayı indir

1. **[Türkçe yamayı indirmek için buraya tıkla — WWE-SvR2011-Turkce-104.zip](https://github.com/ErdemYaziciOfficial/wwe-svr2011-turkce-yama/releases/download/v104/WWE-SvR2011-Turkce-104.zip)**. Dosya yaklaşık **350 MB**.
2. **İndirilenler** klasöründeki `WWE-SvR2011-Turkce-104.zip` dosyasına sağ tıkla → **Tümünü Ayıkla** → **Ayıkla**.
3. Çıkan klasörün içinde **`Kur.ps1`** dosyasını görene kadar klasörleri aç. Uzantılar gizliyse dosya adı **Kur** olarak görünebilir.

**Yama klasörü ve oyun klasörü ayrı kalmalı.** Yama ZIP'ini oyun klasörünün içine çıkarmana veya içindeki dosyaları elle taşıyıp değiştirmenize gerek yok.

> İndirme sayfasını kendin açarsan **Assets** bölümündeki `WWE-SvR2011-Turkce-104.zip` dosyasını seç. **Source code** ve **.sha256** dosyalarını kurulum için indirmene gerek yok.

## 3. Türkçe yamayı kur

**Başlamadan önce oyun ve SvR2011 Launcher kapalı olsun.**

### A. Oyun klasörünün yolunu kopyala

1. Dosya Gezgini'nde **oyunun kurulduğu klasörü** aç. İçinde **`svr2011.exe`** ve **`pac`** klasörü bulunmalı. Az önce indirdiğin yama klasörünü seçme.
2. Pencerenin üstündeki adres çubuğuna tıkla. Klasör yolu yazıya dönüşünce **Ctrl+C** ile kopyala. Örnek: `C:\Oyunlar\SvR2011`.

### B. Yama klasöründe kurucuyu çalıştır

1. **`Kur.ps1` bulunan yama klasörüne** geri dön.
2. Dosya Gezgini'nin üstündeki **adres çubuğuna** tıkla, `powershell` yaz ve **Enter** tuşuna bas. Yeni bir komut penceresi açılır.
3. Aşağıdaki satırın **tamamını** kopyalayıp bu pencereye yapıştır ve **Enter** tuşuna bas. Satırın içinde hiçbir şeyi değiştirmen gerekmiyor:

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File .\Kur.ps1 -OyunKlasoru ((Read-Host 'Oyun klasorunun yolunu yapistir ve Enter tusuna bas').Trim('"'))
```

4. Pencere **oyun klasörünün yolunu** isteyecek. **A bölümündeki oyun klasörüne dönüp adresini tekrar kopyala** (komutu kopyaladığında panonun içeriği değişmişti). Komut penceresine yapıştır ve **Enter** tuşuna bas.
5. Kontroller ve dosya kopyalama bitene kadar bekle. **“Turkce kuruldu”** yazısını görünce kurulum tamamdır; pencereyi kapatabilirsin.

Kurucu, gerekli dosyaları kendisi yerleştirir ve Türkçeyi seçer. Eski dosyalarını oyun klasöründeki **`TR-Yedek-...`** adlı klasöre yedekler. **Bu yedeği silme; yamayı geri almak için gerekiyor.** Oyun kayıtlarına ve ISO dosyana dokunmaz.

## 4. Oyunu aç

Oyunu daha önce açtığın **SvR2011 Launcher** üzerinden başlat. Türkçe yama artık kurulmuş olmalı.

Dil seçmek istersen ana menüden **BENİM WWE → SEÇENEKLER → DİL → TÜRKÇE** yolunu izle. Menü hâlâ İngilizceyse aynı yol **MY WWE → OPTIONS → LANGUAGE → TÜRKÇE** şeklindedir. **Dili değiştirdikten sonra oyunu tamamen kapatıp yeniden aç.**

## Takıldım, ne yapmalıyım?

| Gördüğün durum | Yapman gereken |
|---|---|
| `Kur.ps1` dosyasını bulamıyorum | ZIP'e sağ tıklayıp **Tümünü Ayıkla** işlemini yap. Çıkan klasörün içindeki bir alt klasörde olabilir. |
| “Oyun klasoru bulunamadi” | Yama klasörünü değil, içinde `svr2011.exe` ve `pac` bulunan **asıl oyun klasörünü** seç. |
| “Oyun acik” / “Baslaticiyi kapat” | Oyunu ve başlatıcıyı kapat, kurulum komutunu yeniden çalıştır. |
| “Uyumsuz veya eski yamali temel dosya” | Eski bir yama orijinal dosyaları değiştirmiş olabilir veya oyun sürümün farklıdır. Önce eski yamanın kendi geri alma yöntemiyle orijinale dön. Bu kontrolde kurucu oyuna dosya yazmaz. |
| “Paket bozuk” | Türkçe yama ZIP'ini yeniden indir ve yeni bir klasöre çıkar. |
| Dil değişmedi | Oyunu tamamen kapatıp yeniden aç. Yalnız ana menüye dönmek yeterli değildir. |

**Eski Türkçe yamayı kullanıyorsan:** İngilizce dosyaların üzerine yazan eski yamayı, o yamayla gelen yedek/geri alma yöntemiyle kaldırdıktan sonra bu paketi kur.

**Sonradan PC portunu güncellersen:** güncelleme Türkçe paketin çalıştırıcılarını değiştirebilir. Bu yamanın yeni port sürümüyle uyumu doğrulanmadan güncelleme yapma.

<details>
<summary><strong>Yamayı kaldırmak / önceki hâline dönmek istiyorum</strong></summary>

1. Oyunu ve başlatıcıyı kapat.
2. Oyun klasöründeki, bu kurulumda oluşturulan `TR-Yedek-...` klasörünü aç. Adres çubuğundaki tam yolunu kopyalamak üzere hazır tut.
3. `Geri-Al.ps1` bulunan yama klasöründe adres çubuğuna `powershell` yazıp Enter'a bas.
4. Şu komutu çalıştır; yol sorulduğunda **yedek klasörünün** adresini tekrar kopyalayıp yapıştır:

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File .\Geri-Al.ps1 -YedekKlasoru ((Read-Host 'TR-Yedek klasorunun tam yolunu yapistir').Trim('"'))
```

Önceki çalıştırıcılar ve ayarlar geri gelir. Türkçe dil dosyaları diskte kalabilir; eski çalıştırıcı bunları kullanmaz.

</details>

<details>
<summary><strong>Teknik bilgiler ve dosya doğrulaması</strong></summary>

- Paket: **104**. PC portu tabanı: **2.0.6**, `b4884ac95884406b9b51157479de5a228888fc83`.
- Diğer port sürümleri için uyumluluk garantisi verilmez. Kurucu temel dosyaları ve paket içeriğini SHA-256 ile denetler.
- Türkçe kaynaklar `Mods/Languages/tr-TR` içine kurulur. Eski çalıştırıcıya yalnız `Mods` klasörünü kopyalamak yeterli değildir.
- Komuttaki `ExecutionPolicy Bypass` yalnız açılan PowerShell işlemi içindir; bilgisayarın kalıcı yürütme politikasını değiştirmez. Kurum kısıtlamaları varsa sistem yöneticine danış.
- İsteğe bağlı ZIP doğrulaması: `Get-FileHash .\WWE-SvR2011-Turkce-104.zip -Algorithm SHA256`. Sonucu Release sayfasındaki `.sha256` dosyasıyla karşılaştır.
- Paket, çevrilmiş oyun kaynakları ve uyumlu çalıştırıcı/DLL dosyaları içerir; ISO ve kullanıcı kayıtları içermez.

</details>

## Kapsam ve bilinen sınırlar

- Menü/hikâye çevirileri, PC arayüzü ve Türkçe font desteği paket içindedir.
- John Cena'nın ilk MVP maçından sonraki RTWM sahnesinde bildirilen karakter hatasının düzeldiği kullanıcı tarafından doğrulandı.
- Özel adlar, hareket adları, teknik/ses kimlikleri ve Dummy/Text yer tutucuları çeviri hedefi değildir. Bu kayıtlar çevrilmiş olarak sayılmaz.
- Görsellere gömülü kalan İngilizce yazılar ertelendi. Önceden kurulmuş YENİ/HAZIR texture paketleri korunur ancak bu arşive dahil değildir.
- Bu sürüm için baştan sona yeni bir oyun/RTWM oynanışı testi yapılmadı; **%100 çeviri veya hatasızlık iddiası yoktur**.
- Dil ekranı, İngilizce/Türkçe arasında seçim ve yeniden başlatma, iki dilde 60'ar dosya okuma, kurulum/geri alma ve bozuk paket engeli doğrulandı.

![Türkçe dil seçeneği](turkce.png)

## Kaynak ve katkılar

Bu bağımsız fan yamasının yönetimi ve oyun içi geri bildirimi **ErdemYaziciOfficial**, AI destekli çeviri ve teknik uygulaması **OpenAI Codex** ile yapılmıştır. PC portunun ve altyapıların tüm katkıları [CREDITS.md](CREDITS.md) içindedir. Kaynak değişiklikleri ve üçüncü taraf bildirimleri Release paketinde bulunur. Orijinal oyun, port ve üçüncü taraf bileşenlerinin hakları sahiplerine aittir; tüm pakete tek bir lisans atanmamıştır.
