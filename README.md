# efmon (scroll down for English)
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

Örnek kullanım: ```efmon -b wlan0```
Örnek kullanım 2: ```efmon --kapat -w wlan0mon```
NOT: efmon wlan0 komutu monitor mod başlatır aynı, -b yazmışsınız gibi.

# Kullanım:
Ana kodu Kali Linux içerisinde '/bin' içine atmanız yeterlidir
Komutlar sırasıyla:
```
git clone https://github.com/K4hveci/efmon
mv efmon /bin
```

Not: "airmon-ng" yoksa bile '-w' parametresi ile 'iwconfig' üzerinden monitor mod kullanabilirsiniz.

# efmon
A simple Kali Linux tool to switch to monitor mode or stop monitor mode


#             efmon v1.0                               
efmon: This tool is designed to easily enable and disable monitor mode.
To use it, simply type efmon and specify the device/interface with a parameter.
This tool uses airmon-ng.

-h/--help: Prints this help message.
-b/--baslat:(start) Parameter to enable monitor mode.
-k/--kapat:(stop/close) Parameter to disable monitor mode.
-d/--durum:(status) Parameter to check if monitor mode is enabled or disabled.
-w/--iwconfig: Starts monitor mode using 'iwconfig' instead of 'airmon-ng'.

Example usage: ```efmon -b wlan0```
Example usage 2: ```efmon --stop -w wlan0mon```
NOTE: The 'efmon wlan0' command starts monitor mode just as if you had typed -b.

# Usage:
Place the main code into the '/bin' directory within Kali Linux.
The commands are as follows:

```
git clone https://github.com/K4hveci/efmon
mv efmon /bin
```
Note: Even if "airmon-ng" is not available, you can use monitor mode via 'iwconfig' with the '-w' parameter.
