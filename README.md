# Pardus AutoSetup 
## **Pardus Otomatik Kurulum Aracı**
![Pardus Resim](https://www.ankarakreatif.com/uploads/haberler/1534682669pardus-isletim-sistemi-png.png)

## **Pardus AutoSetup Nedir?**

Live ya da normal kurulum sonrası açılan Pardus'a otomatik olarak belirlediğim uygulamaları indiren ve ayarlarımı yapan bir BASH Scripttir.

## **Nasıl Çalışır?**

 Ana dizinde bulunan kurulum başlatıcılarından, kullandığınız Pardus dağıtımına göre çalıştırınız.

 XFCE Kurulum:
 ```bash
 bash setupXFCE.sh
 ```
 Gnome Kurulum:
```bash
bash setupGnome.sh
```
## **Kullanmadan Önce Yapmanız Gerekenler**

- İndireceğiniz uygulamaların adlarını koda benzer şekilde eklemek ya da silmek.

## **Hata Anında Ne Yapmalıyım?**
 
 Uygulama içi hata vermemek adına sürekli apt onarılıyor ve güncelleniyor. Fakat bazı iptal etme durumlarında apt arızalanabiliyor.

 Eğer,
 ```
E: /var/lib/dpkg/lock kilidi alınamadı - open (11: Özkaynak geçici olarak kullanılamaz durumda)

E: Yönetim dizini (/var/lib/dpkg/)kilitlenemiyor, başka bir işlem tarafından kullanılıyor olmasın?
```
hatasını alırsanız repair klasöründe bulunan apt-lock-error-solve.sh dosyasını çalıştırın.

Bağımlılık hatası aldığınızda ise apt-repair.sh'ı çalıştırabilirsiniz.

## **VSCode Ve Discord'u Güncellemek**

Bunun için parXFCE ya da parGnome dosyasının içinden oto indirilen dosya adını kopyalayıp koda entegre edin. (İleride giderilecek.)

Ömer Ayyıldız
