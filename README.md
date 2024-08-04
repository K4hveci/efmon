# efmon
 Monitor moda geçmek veya monitor modu durdurmak için basit bir Kali Linux aracı
    
                  efmon v1.0                               

efmon: Bu tool monitör modu kolayca açıp kapatabilmeniz içindir.
Kullanım için efmon yazmanız ve parametre ile cihaz/interface belirlemeniz yeterlidir.
Bu tool airmon-ng kullanmaktadır.

-h/--help:  Bu yardım mesajını yazdırır.
-b/--baslat: Monitro modu başlatmak için girmeniz gereken parametre.
-k/--kapat: Monitor modu kapatmak için girmeniz gereken parametre.
-d/--durum: Monitor modun açık veya kapalı olduğunu görmeniz için girmeniz gereken parametre.
-w/--iwconfig: Monitor modu 'airmon-ng' yerine 'iwconfig' ile başlatır.

Örnek kullanım: 'efmon -b wlan0' 
Örnek kullanım 2: 'efmon --kapat -w wlan0mon'
NOT: efmon wlan0 komutu monitor mod başlatır aynı, -b yazmışsınız gibi.

# Kullanım:
Ana kodu Kali Linux içerisinde '/bin' içine atmanız yeterlidir
Komutlar sırasıyla:
```
git clone https://github.com/K4hveci/efmon
mv efmon /bin
```

Not: "airmon-ng" yoksa bile '-w' parametresi ile 'iwconfig' üzerinden monitor mod kullanabilirsiniz.
