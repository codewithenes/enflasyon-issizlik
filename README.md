# enflasyon-issizlik
Enflasyon ve İşsizlik Tablosundaki bozuk verileri düzenleme
* 2006 - 2019 arası işsizlik ve enflasyon değerlerini gösteren veritabanında NaN değerler, bozuk ve aykırı değerler varmı varsa bunların düzenlenmesi gerekmesi sonucu Dataseti inceledim.
* Öncelikle gerekli kütüphaneleri ve data dosyasını import ettim.
* Verileri incelediğimde Aykırı veya Bozuk değere rastlamadım fakat NaN veya Null olarak nitelendirilen Boş kayıtlar buldum ve Enflasyon ve İşsizlik isimli 2 tablo ise float değerinde olması gerekirken Object yani string değerdeydi.
* öncelikle yanlış veri tiplerini astype fonksiyonu ile düzelttim.
•sonrasında dropna fonksiyonu ile NaN değerleri sildim ve bunun kalıcı olması için inplace=True komutunu kullandım.
* yazdığım tüm kodlara ve dataya mevcut github dosyasından ulaşabilirsiniz.
* bir sonraki güncellemede mevcut dataların arasındaki (varsa) bağlantıyı inceleyip bulgu kısmını ekleyeceğim.

* Güncelleme
* Elde ettiğim datayı korelasyon kontrolü için kullanılan corr fonksiyonu başta olmak üzere birçok matematiksel fonksiyon ile inceledim.
* Korelasyon 0.194711 Çıktı bunun anlamı Çok ufak neredeyse kayda değer bile olamayacak şekilde Pozitif bir korelasyon olduğunu gösteriyor.
* Seaborn Kütüphanesi ile grafik şeklinde projede görebilirsiniz.
* Çıkan sonuç 'Phillips eğrisi' teorisine uygun şekilde çıkmadı.
