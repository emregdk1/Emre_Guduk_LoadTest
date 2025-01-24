# Emre_Guduk_LoadTest

JMeter Test Plan: HomePage.jmx

# Proje Açıklaması

Bu proje, Apache JMeter kullanılarak oluşturulmuş bir yük testi planını içermektedir. HomePage.jmx, web uygulamasının ana sayfa performansını ve yük altındaki davranışını test etmek amacıyla tasarlanmıştır. Test senaryosu, ana sayfanın çeşitli kullanıcı istekleri altında nasıl tepki verdiğini ölçmeyi hedefler.

# Başlarken

Bu projeyi kullanmaya başlamadan önce JMeter'ın sisteminizde kurulu olduğundan emin olun. Aşağıdaki adımları takip ederek bu dosyayı çalıştırabilirsiniz.

# Gereksinimler

Apache JMeter (versiyon 5.4.3 veya üstü önerilir)

Java (JDK 8 veya üstü)

JMeter ile uyumlu bir sistem (Windows, macOS veya Linux)

# Kurulum

Apache JMeter indirin ve kurun.

HomePage.jmx dosyasını bu projeden indirin veya klonlayın.

# Kullanım

Apache JMeter'ı başlatın:

jmeter

File > Open menüsünden HomePage.jmx dosyasını seçin.

Test planını inceleyin ve gereksinimlerinize göre özelleştirin.

Testi çalıştırmak için üst menüden Start butonuna basın.

# Komut Satırından Çalıştırma

JMeter test planını komut satırından çalıştırmak için şu adımları izleyin:

# jmeter -n -t HomePage.jmx -l results.jtl" #

-n: Non-GUI (Grafik Arayüzsüz) modunda çalıştırır.

-t: Test planı dosyasının yolunu belirtir.

-l: Test sonuçlarının kaydedileceği dosya yolunu belirtir.

# Sonuç Analizi

Test sonuçlarını JMeter GUI üzerinden inceleyebilirsiniz.

Results Tree veya Summary Report kullanarak detaylı analiz yapabilirsiniz.

## Test Planı Detayları

# HomePage
Bu test planı aşağıdaki HTTP isteklerini içermektedir:

# Note: "/-438" adlı servis üzerinde JMeter kullanılarak URL doğrulaması gerçekleştirilmiştir.

URL: /-438

Method: GET

Açıklama: Ana sayfa yükleme isteği.

URL: /live-chat

Method: GET

Açıklama: Canlı destek bileşeni.

URL: /hesabim/hesap-bilgileri

Method: GET

Açıklama: Kullanıcı hesap bilgileri sayfası.

URL: /component/render/conceptPromotion

Method: GET

Açıklama: Konsept promosyon bileşeni.

URL: /events

Method: OPTIONS ve POST

Açıklama: Event API üzerinden veri alışverişi.

URL: /eventhandler/n11/web

Method: POST

Açıklama: Özel event işleme.

URL: /component/render/homepageRecommendation

Method: GET

Açıklama: Ana sayfa öneri bileşeni.


# Test Planı Detayları

# Search

# Note: "/arama/tamamla-358" servisi üzerinde JMeter kullanılarak aramaya yazılan değerin doğrulaması gerçekleştirilmiştir.

Bu test planı aşağıdaki HTTP isteklerini içermektedir:

URL: /arama

Method: GET

Açıklama: Arama sorgusu gönderir.

URL: /live-chat

Method: GET

Açıklama: Canlı destek erişimi.

URL: /hesabim/hesap-bilgileri

Method: GET

Açıklama: Kullanıcı hesap bilgileri.

URL: /web-store-chat

Method: POST

Açıklama: Web mağazası sohbet isteği.

URL: /eventhandler/n11/web

Method: POST

Açıklama: Event işleme servisi.

URL: /events

Method: POST

Açıklama: Genel event işlemleri.

URL: /arama/tamamla

Method: GET

Açıklama: Arama tamamlayıcı servis.
