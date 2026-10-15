**Bu dosya, web-projesi (Ortak Gider Takipçisi) projesinde yapay zekanın nerede, nasıl ve ne kadar kullanıldığını kayıt altına alır.**
	
*Kullanılan araç:	claude.ai 
*Kullanım tarihi:	15.10.2026
*Proje	webb: ortak harcamaları takip eden web uygulaması
*Kullanım amacı:	Fikir bulma, prototip kodu


**Sorduğum:** [README]'de yazdığım problemleri karşılayacak özellikte bir şeyler yapabilir misin? Ardından, projede yapmamız gereken diğer şeyleri de hazırlamasını istedim.
**Aldığım cevap:** HTML, CSS ve JavaScript'in tek dosyada olduğu bir prototip. Kişi ekleme, harcama ekleme/düzenleme/silme, kişi başı pay hesabı, kim kime ödeyecek hesabı ve tarayıcıda veri saklama içeriyor.

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
