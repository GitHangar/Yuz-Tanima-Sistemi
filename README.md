# Yüz Tanıma Sistemi
![demo](https://github.com/SuleymanKaya1/Yuz-Tanima-Sistemi/blob/main/demo.png)<br>
İnsanların sadece bir fotoğrafını kullanarak bilgisayar ortamında onları tanımak mümkün. Bilgisayarınız tarafından tanınması istediğiniz kişilerin fotoğraflarını 'PersonelYuzleri' klasörünün içine atın ve yazılımı çalıştırın; canlı olarak kameradan yüz tanımak işte bu kadar basit. Tanınan yüzleri ise saat kaçta tanıdığını Kayıtlar.csv adlı dosyaya kaydediyor, böylelikle personel/şahısların giriş çıkış saatleri belirlenebiliyor.
## Kurulum
### Windows:
1. [Buradan](https://git-scm.com/download/win) Git'i indirin ve kurun
2. [Buradan](https://github.com/Kitware/CMake/releases/download/v3.20.1/cmake-3.20.1-windows-x86_64.msi) CMake aracını indirin ve kurun (C derleyicisine ihtiyaç duyduğumuz için bu yazılımı kullanıyoruz)
3. [Buradan](https://visualstudio.microsoft.com/tr/thank-you-for-downloading-visual-studio-for-cplusplus/?sku=Community&rel=16&rid=30005) Visual Studio C++ indirin ve kurun (C++ derleyicisine ihtiyaç duyduğumuz için bu yazılımı kullanıyoruz) 
4. Komut istemini (CMD) yönetici olarak çalıştırın, ardından komut isteminde şu komudu çalıştırın:
```
git clone https://github.com/SuleymanKaya1/Yuz-Tanima-Sistemi.git && cd Yuz-Tanima-Sistemi && pip install -r gereksinimler.txt
```

### Linux (Debian / Ubuntu Tabanlı Dağıtımlar):

```bash
git clone https://github.com/SuleymanKaya1/Yuz-Tanima-Sistemi.git && cd Yuz-Tanima-Sistemi && sudo apt install cmake g++ && pip3 install -r gereksinimler.txt
```
İşletim sisteminize uygun olan adımları başarılı bir şekilde gerçekleştirdiyseniz yazılım hatasız çalışacaktır.

## Yazılım Nasıl Kullanılır?
1. Personellerin vesikalık fotoğrafını çekin
2. Çektiğiniz fotoğrafları kişilerin ismiyle yeniden adlandırın
3. Fotoğrafları 'PersonelYuzleri' klasörünün içine atın

Örnek olarak X kişisini algılayalım:
1. X kişisinin vesikalık fotoğrafını çekin
2. Çektiğiniz fotoğrafı X.jpg olarak yeniden adlandırın.
3. Bu fotoğrafı 'PersonelAlgilama' isimli klasöre aktarın

Ardından işletim sisteminizin komut satırında yazılımı çalıştırın.
### Windows:
```
python KameradanPersonelAlgilama.py
```
### Linux:
```
python3 KameradanPersonelAlgilama.py
```

## Yüz Karşılaştırma Yazılımı
Tıpkı filmlerdeki gibi iki insan aynı kişi mi değil mi karşılaştırmayı sağlayan yazılım. Bunu çalıştırmak içinse yapmanız gereken şeyler şunlardır:
1. Kişinin resmini 'fotograf1.jpg' olarak yeniden adlandırın
2. Karşılaştırmak istediğiniz kişinin resmini 'fotograf2.jpg' olarak yeniden adlandırın
3. Bu iki dosyayı 'YuzKarsilastirmaKlasoru'ne atın ve Yüz Karşılaştırma Yazılımını çalıştırın
### Windows:
```
python YuzKarsilastirma.py
```
### Linux:
```
python3 YuzKarsilastirma.py
```
## Nasıl Katkı Sağlarım?
Bir pull request harika olur :) Büyük değiştirmeler için lütfen yapacağınız değiştirme hakkında konu açın.

Lütfen testleri uygun şekilde güncellediğinizden emin olun.

## Lisans
[GPLv3](http://www.gnu.org/licenses/gpl-3.0.tr.html)
