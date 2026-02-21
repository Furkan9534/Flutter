# Flutter

## Mobil Geliştirme Yaklaşımları
Mobil uygulama geliştirirken 3 tür mobil geliştirme yaklaşımı vardır. Bunlar : 
-Native
-Hybrid
-Cross Platform

# Native Yaklaşım

Native yaklaşım, bir mobil uygulamanın doğrudan hedeflediği işletim sistemine (IOS , Android) özgü diller ve araçlar kullanılarak geliştirilmesidir. Örneğin IOS için swift ve objective C , Android için ise Kotlin ve Java kullanılır. Bu yaklaşımda , kodlar doğrudan işlemcinin anlayacağı makine diline derlenecektir.Bu yüzden veri işleme, tepki süreleri en hızlı ve üst seviye de olur. 

Kamera , GPS , Bluetooth ve sensörler gibi cihaz özelliklerine herhangi bir köprü (bridge) olmadan sorunsuz ve doğrudan çalışmamıza imkan sunar. Apple ve Google sahip olduğu appstore da tasarım ve özelliklere hemen uyum sağlar. 

| Flutter Avantajlar  | Flutter Dezavantajlar |
| -------------       | ------------- |
| Kullanıcı Deneyimi  | IOS ve Android için iki ayrı geliştirici ve ekip gerekir.  |
| İntennet bağlantısı olmadan verilmli çalışma | Her iki platform için ayrı ayrı geliştirme yapma zorunluluğu. |
| Karmaşık hesaplamalar ve yoğun grafikli (oyun vb.) işler için idealdir.|Bir hata düzeltildiğinde iki farklı kodun da güncellenmesi gerekir. |

# Hybrid Yaklaşım

Mobil uygulama geliştirirken web teknolojileri ile (HTML,CSS,Javascript) ile yerel (native) uygulama özelliklerini bir araya getiren "melez" bir yöntemdir. Temelde bir web sitesi gibi kodlanan uygulamanın, "Native Wrapper" adı verilen yerel bir kabuk içine yerleştirilerek uygulama mağazalarında (App Store, Google Play) yayınlanabilmesini sağlar.

### Hibrit Yaklaşımın Temel Özellikleri
-Uygulama bir kez yazılır; aynı kod hem Android hem de iOS üzerinde çalışır. \
-Geliştirme sürecinde JavaScript, HTML5 ve CSS gibi standart web dilleri kullanılır. \
-Kamera, rehber veya GPS gibi donanımsal özelliklere özel eklentiler (pluginler) aracılığıyla erişebilir. \
-Güncellemeler tek bir yerden yapıldığı için yönetim ve bakım süreçleri daha hızlıdır. \






---