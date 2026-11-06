**Bu dosya, web-projesi (Ortak Gider Takipçisi) projesinde yapay zekanın nerede, nasıl ve ne kadar kullanıldığını kayıt altına alır.**
	
*Kullanılan araç:	claude.ai 
*Kullanım tarihi:	15.10.2026
*Proje	web: ortak harcamaları takip eden web uygulaması
*Kullanım amacı:	prototip kodu


** Soru - Cevap Kayıtları

#** 1. Proje problemi
**Sorduğum soru:**
> bana günlük hayattan bir problemden bahset

**Verilen cevap:**
Yapay zeka web ile çözülebilecek 5 problem önerdi: ortak giderleri takip edememek, ders ve ödev tarihlerini kaçırmak, yemek israfı, çalışma zamanını verimsiz kullanmak ve yemekhane menüsüne ulaşamamak. Kendi yaşadığım bir sıkıntıyı seçmemi önerdi.

**Nasıl kullandım:** Listeden ortak gider takibini seçtim.

### 3. Prototip
**Sorduğum soru:**
> bahsettiğin bu özellikleri yapabilecek misin

**Verilen cevap (özet):**
Evet, tek dosyalık `index.html` ile yapılabileceğini söyledi. Kişi ekleme, harcama ekleme, kişi başı pay hesabı, borç durumu ve silme/düzenleme özelliklerini sayıp, bunun giriş sistemi ve veritabanı olmayan bir prototip olacağını belirtti.

**Nasıl kullandım:** Verilen `index.html` dosyasını repoya yükledim ve GitHub Pages ile yayınladım.

### 4. GitHub Pages
**Sorduğum soru:**
> save atmama izin vermiyor

**Verilen cevap (özet):**
Save butonunun gri olmasının Pages'in zaten açık ve kayıtlı olduğunu gösterdiğini, sitenin `2kalayci.github.io/web-projesi/` adresinde açılacağını söyledi.

**Nasıl kullandım:** Adresi açıp sayfanın çalıştığını kontrol ettim.

**Test ettiklerim:**
* 2-3 kişi ekleyip birkaç harcama girdim, sonuçlar doğru çıktı.
* Elle hesapladığım sonuçla karşılaştırdım.
* Düzenleme ve silme çalışıyor.
* Sayfayı yenileyince veriler duruyor.
* Telefonda / dar ekranda açıp baktım.
* Kodu olduğu gibi kullandım.

**Kodun mantığı**
Her kişinin bakiyesi = ödediği toplam tutar − kişi başı pay. Pozitifse alacaklı, negatifse borçludur.
Kişi başı pay = toplam harcama ÷ kişi sayısı.
Kim kime ödeyecek: En çok borçlu kişi, en çok alacaklı kişiye ödeme yapar. Biri sıfırlanınca sıradakine geçilir. Böylece hesap en az ödemeyle kapanır.

**Önem verdiğim şeyler**
Uygulama harcamaları herkes arasında eşit böler. Farklı pay oranları desteklenmiyor.
Veriler sadece kullanıcının tarayıcısında tutulur, sunucu veya giriş sistemi yoktur.
Yapay zekanın yazdığı kodu körü körüne kullanmadım, çalıştırıp sonuçları kontrol ettim.
Yapay zeka hata yapabilir. Bu yüzden hesaplama sonuçlarını elle de doğruladım.

**Yapay zekayı yardımcı araç olarak kullandım. Çıktıları okudum, test ettim ve projeye kendi kararlarımla uyarladım.**
