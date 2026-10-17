# UYAP-Editor-5.4.20
UYAP Editor 5.4.20
Degisiklikler:
- Dort .ini dosyasinda Minimum Version 1.8 yerine 11 yapildi.
- JVM parametrelerine su paketler icin --add-opens=MODUL/PAKET=ALL-UNNAMED eklendi:
  java.base/java.util
  java.base/java.lang.reflect
  java.base/java.text
  java.desktop/java.awt.font
  java.desktop/java.awt
- editor_lib.jar icindeki WPAppManager.class dosyasinin private static boolean e()
  surum kontrolunde ust sinir 14 yerine 25 yapildi. Diger JAR dosyalari degismedi.
- Dokuman editorunun .ini dosyasina java25-error.log / java25-output.log yolları eklendi.

Dogrulama:
- Kurulu kutuphanelerle XStream baslatma testi Temurin Java 25.0.4.1 ile gecti.
- Normal Uyap Dokuman Editoru.exe baslaticisi Java 25.0.2 ile editor ekranini acti.
- Kaydetme, tekrar acma, yazdirma, e-imza ve sablon editoru islevleri test edilmedi.
- x86 baslaticilari test edilmedi; kullanilmalari icin 32 bit Java gerekir.
- Eski XStream, sun.misc.Unsafe icin kullanimdan kaldirma uyarisi veriyor.
  Bu uyumluluk duzeltmesi kutuphaneyi modernlestirmez ve Java 25 sonrasi garanti vermez.

UYAP guncelleyicisi JAR veya ayarlari degistirirse bu duzeltme kaybolabilir.
Resmi bir UYAP guncellemesi degildir; bu bilgisayara uygulanan yerel uyarlamadir.

Java --add-opens belgesi:
https://docs.oracle.com/en/java/javase/25/migrate/migrating-jdk-8-later-jdk-releases.html

Resmi indirme linki https://uyap.gov.tr/UYAP-Editor
indirme linkinden indirdiğinizde hata verdiğinde yüklediğim dosyaları C:\Uyap\Uyap Kelime Islemci dosya yoluna atarsanız sorunsuz şekilde çalışacaktır.
