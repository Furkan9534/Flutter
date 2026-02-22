# Flutter

## Mobil Geliştirme Yaklaşımları
Mobil uygulama geliştirirken 3 tür mobil geliştirme yaklaşımı vardır. Bunlar : 
-Native
-Hybrid
-Cross Platform

# Native Yaklaşımı

Native yaklaşım, bir mobil uygulamanın doğrudan hedeflediği işletim sistemine (IOS , Android) özgü diller ve araçlar kullanılarak geliştirilmesidir. Örneğin IOS için swift ve objective C , Android için ise Kotlin ve Java kullanılır. Bu yaklaşımda , kodlar doğrudan işlemcinin anlayacağı makine diline derlenecektir.Bu yüzden veri işleme, tepki süreleri en hızlı ve üst seviye de olur. 

Kamera , GPS , Bluetooth ve sensörler gibi cihaz özelliklerine herhangi bir köprü (bridge) olmadan sorunsuz ve doğrudan çalışmamıza imkan sunar. Apple ve Google sahip olduğu appstore da tasarım ve özelliklere hemen uyum sağlar. 

| Flutter Avantajlar  | Flutter Dezavantajlar |
| -------------       | ------------- |
| Kullanıcı Deneyimi  | IOS ve Android için iki ayrı geliştirici ve ekip gerekir.  |
| İntennet bağlantısı olmadan verilmli çalışma | Her iki platform için ayrı ayrı geliştirme yapma zorunluluğu. |
| Karmaşık hesaplamalar ve yoğun grafikli (oyun vb.) işler için idealdir.|Bir hata düzeltildiğinde iki farklı kodun da güncellenmesi gerekir. |

# Hybrid Yaklaşımı

Mobil uygulama geliştirirken web teknolojileri ile (HTML,CSS,Javascript) ile yerel (native) uygulama özelliklerini bir araya getiren "melez" bir yöntemdir. Temelde bir web sitesi gibi kodlanan uygulamanın, "Native Wrapper" adı verilen yerel bir kabuk içine yerleştirilerek uygulama mağazalarında (App Store, Google Play) yayınlanabilmesini sağlar.

### Hibrit Yaklaşımın Temel Özellikleri
-Uygulama bir kez yazılır; aynı kod hem Android hem de iOS üzerinde çalışır. \
-Geliştirme sürecinde JavaScript, HTML5 ve CSS gibi standart web dilleri kullanılır. \
-Kamera, rehber veya GPS gibi donanımsal özelliklere özel eklentiler (pluginler) aracılığıyla erişebilir. \
-Güncellemeler tek bir yerden yapıldığı için yönetim ve bakım süreçleri daha hızlıdır. \

### Hybrid Yaklaşımın Avantaj ve Dezavantajları

| Özellik  | Hibrit Yaklaşım |
| ------------- | ------------- |
| Maliyet  | Tek kod yazıldığı için daha ekonomiktir.|
| Geliştirme Hızı  | Pazara çıkış süresi oldukça kısadır.|
| Performans | Native yaklaşım uygulamalarına göre daha yavaştır.|
| Kullanıcı Deneyici |Karmaşık animasyonlarda ve geçişlerde akıcılık sorunları yaşanabilir.|

### Hybrit Yaklaşım Araçları
 En yaygın kullanılan platformlar arasında Ionic, Cordova ve PhoneGap kullanılmaktadır. 

### Cross Platform Yaklaşımı

Cross Platformun anlamı çarpraz platform anlamına gelmektedir. Mobil uygulamada native yaklaşımda her platform için ayrı dillerde ayrı uygulamalar geliştirirken , cross platform sayesinde geliştiriciler kodun büyük kısmını ortak yazıp her iki platform için kullanabiliyorlar. 

### Cross Platform Yakşalım Avantajları ve Dezavantajları

| Avantajlar   | 	Dezavantajlar |
| ------------- | ------------- |
| Maliyet, tek ekip ve tek kod tabanı ile maliyetler düşecektir. |Performans, native uygulamalara göre biraz daha yavaştır.|
| İki platforma da aynı anda girilebileceği için pazara giriş hızlanır.  |Donanım Erişimi: En yeni cihaz özelliklerine veya sensörlere erişim için bazen güncellemeleri beklemek gerekebilir.|
| Hata düzeltmeleri veya güncellemeler tek merkezden yapılır. | Kullanıcı deneyimi açısından iki platformunda kendine has dillerine tam uyum sağlaması zor olabilir.|

### En Popular Cross Platform Araçları

| Araçlar  | 
| ------------- |  
| Flutter (Google)  |  
|React Native  |  
| Kotlin Multiplatform  |   
 

### Flutter'ı diğer frameworklerden ayıran ve onu benzersiz yapan temel fark nedir ? 

Flutter'ı benzersiz yapan temel fark cihazın kendi arayüz bileşenlerini kullanmak yerine her bir pikseli ekrana kendisinin çizmesidir. 

### Flutter'ı rakiplerinden ayıran başlıca özellikler : 

1. Kendi Grafik Motoru (Skia / Impeller)

Geleneksel çarpraz platform araçları , cihazın kendi butonlarını , metin kutularını kullanmak için bir köprü (bridge) kurar. Flutter ise Skia veya yeni nesil impeller sayesinde  tüm arayüzü doğrudan GPU üzerinden çizer.

2. "Her Şey Bir Widget'tır"
Flutter'da   butonlar, listeler , hizalamalar (padding), temalar ve hatta navigasyon bile birer widget'tır. Bu sayede geliştiricilere geliştirmeleri için sınırsız bir özelleştirme gücü verir.  

3. Gerçek Native Performans

Flutter, Dart kodunu doğrudan cihazın işlemcisinin anlayacağı makine koduna (ARM) derler. 

4. Gelişmiş Geliştirici Deneyimi (Hot Reload)
Uygulamada koddaki yaptığınzı değişiklikleri anında ekranda görmenizi sağlar. Hot Reload özelliği, geliştirme sürecini native yöntemlere göre 3 kata kadar hızlandırabilir.

5. Tek Kod
Flutter, sadece mobil uygulama için değildir. Aynı kod tabanı ile hiçbir performans kaybı yaşamadan Web, Windows, macOS, Linux ve hatta gömülü sistemler için uygulama çıktıları alınabilir.

### StatelessWidget(Durumsuz Widget) ve StatefulWidget (Durumlu Widget)

Stateless widget'lar, uygulamada oluşturulduktan değişmeyen, sabit ve statik bileşenlerdir. Bir kez render edildikten sonra kendi içlerinde bir durumu güncelleyemezler.

-Kullanım Amacı : Kullanıcı tarafından değişmeyecek  sadece bilgi gösteren sabit yapılar için kullanılır. Text, icon , resim örnek verilebilir. 

 Stateful Widget'lar ise uygulama çalışırken dinamik olarak çalışan etkileşimli bileşenlerdir. Kullanıcı bir işlem yaptığında veya veri değiştirildiğinde setState() metodu sayesinde ekranın ilgili kısmını yeniden çizerler. 
 
 -Kullanım Amacı : Kullanıcı tarafından girilen verilere göre, zamanla değişebilen yapılardır.


| Özellik  | StatelessWidget | StatefulWidget |
| ------------- | ------------- |
| Durum  | Tek kod yazıldığı için daha ekonomiktir.|
| Yapı  | Pazara çıkış süresi oldukça kısadır.|
| Metod | Native yaklaşım uygulamalarına göre daha yavaştır.|
| Performans |Karmaşık animasyonlarda ve geçişlerde akıcılık sorunları yaşanabilir.|



---