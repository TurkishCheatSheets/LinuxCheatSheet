```bash
.____    .__                      _________ .__                   __      _________.__                   __
|    |   |__| ____  __ _____  ___ \_   ___ \|  |__   ____ _____ _/  |_   /   _____/|  |__   ____   _____/  |_
|    |   |  |/    \|  |  \  \/  / /    \  \/|  |  \_/ __ \\__  \\   __\  \_____  \ |  |  \_/ __ \_/ __ \   __\
|    |___|  |   |  \  |  />    <  \     \___|   Y  \  ___/ / __ \|  |    /        \|   Y  \  ___/\  ___/|  |
|_______ \__|___|  /____//__/\_ \  \______  /___|  /\___  >____  /__|   /_______  /|___|  /\___  >\___  >__|
        \/       \/            \/         \/     \/     \/     \/               \/      \/     \/     \/

```

[comment]: <> (LinuxCheatSheet yazisi kaldirilsa daha mi iyi olur?)

# Linux Cheat Sheet

## Dosya Komutları

```bash
$ cat filename
   # dosya içeriğini gösterir.
```

```bash
$ cat > filename
   # Dosyaların standart girişten listelenmesi
```

```bash
$ cd
   # Dizini değiştirmek için kullanılan komut
```

```bash
$ cmp
   # Herhangi iki tür dosyayı karşılaştırır ve sonucu standart çıktıya yazar.
   # Eğer dosyalar aynıysa öntanımlı olarak cmp komutu birşey yapmaz.
   # Eğer farklıysalar, ilk farkın oluştuğu bayt ve satır sayısı gösterilir.
```

```bash
$ cp originalfilename newfilename
   # dosya ve dizinleri kopyalar
```

```bash
$ cut
   # girişin herbir satırındaki bölümleri alıp ekranda gösterir
```

```bash
$ diff
   # Bilgisayar ile hesaplamada bir dosya karşılaştırma yardımcı programıdır ve iki dosya arasındaki farkları bulmaya yarar.
```

```bash
$ join
   # iki dosyanın satırlarını ortak bir alanda birleştirir.
```

```bash
$ ls -l
   # dosyalar hakkında bilgi listeler
```

```bash
$ ls -la
   # dosyalar hakkında bilgi listeler gizli dosyalarda dahil
```

```bash
$ mkdir
   # yeni bir dizin oluşturur
```

```bash
$ mv
   # belirtilen dosyayı yeniden adlandırır yada taşımaya yarar
```

```bash
$ nl
   # satır sayısını gösterir.
```

```bash
$ touch filename
   # yeni bir dosya oluşturma
```

```bash
$ pwd
   # içinde bulunduğu dizinin ismini gösterir
```

```bash
$ rm -rf dirname
   # dosya ve dizinleri siler
```

```bash
$ wc
   # Kelime Sayma İşlemlerini Gerçekleştiren Komuttur
```

```bash
$ ln -s filename link
   # sembolik link oluşturur.
```

```bash
$ head
   # Her DOSYA'nın ilk on satırını standart çıktıya yazar.
```

```bash
$ tail
   # Belirtilen her DOSYA'nın son 10 satırını standart çıktıya yazar.
```

```bash
$ tail -f
   # Belirtilen her DOSYA'nın son 10 satırını sürekli izleyerek standart çıktıya yazar.
```

## SSH & Güvenli Dosya İşlemleri

```bash
$ scp dosyaadi kullaniciadi@uzaksunucu:/home/
   # uzak sunucuya güvenli bir şekilde dosya aktarımına yardımcı olur.
```

```bash
$ sftp
   # Dosya transferi için alternatif bir uygulama
```

```bash
$ ssh user@host
   # sunucuya kullanıcı adınız ile giriş yapabilirsiniz.
```

```bash
$ ssh -p user@host
   # özel tanımlanan port numarası ile sunucuya kullanıcı adınız ile giriş yapabilirsiniz.
```

```bash
$ ssh-copy-id user@host
   # şifre olmadan ssh key aracılığı ile giriş yapmayı etkinleştirir.
```

## Süreç Yönetimi

```bash
$ ps
   # Aktif olan tüm işlemleri gösterir(bash,root,su vb)
```

```bash
$ top
   # Çalışan sistemdeki tüm işlemleri gösterir
```

```bash
$ kill pid
   # Çalışan bir uygulamayı pid numarasına göre sonlandırır.
```

```bash
$ killall proc
   # proc ile başlatan tüm işlemleri sonlandırır.
```

```bash
$ bg
   # arka plandaki işlerin tamamını durdurur.
```

```bash
$ renice
   # çalışan işlemlerin önceliğini değiştirmek için kullanılır.
```

## Grup & Dosya İzinleri

```bash
$ chmod
   # dosyanın iznini değiştirmeye yarar
```

```bash
$ chgrp
   # grup-id ye göre grup izinlerini değiştirmeye yarar.
```

```bash
$ groups
   # grup üyeliklerinde değişiklik
```

## Arama Komutları

```bash
$ grep [pattern] dosya
   # belirtilen pattern göre dosyalarda arama yapar.
```

```bash
$ grep -r [pattern] klasör
   # özyenileme yöntemi ile dizin içerisinde arama yapar
```

```bash
$ find dosya
   # dosyanın tüm örneklerini bulmaya yarar.(UNİX)
```

```bash
$ locate dosya
   # dosyanın tüm örneklerini bulmaya yarar.
```

```bash
$ xargs
   # argüman listesi oluşturmaya yarar.Oluşturulan bu listeye görede başka komutlar tetikler
```

## Sıkıştırma Komutları

```bash
$ tar -xf dosyaadi.tar
   # dosyaadi.tar içerisindeki dosyaları çıkartır
```

```bash
$ tar -cf dosyaadi.tar dosyaadi
   # dosyaadi.tar şeklinde sıkıştırılmış dosya oluşturur.
```

```bash
$ tar -czf dosyaadi.tar.gz
   # gzip kullanarak dosyaadi.tar.gz oluşturur.
```

```bash
$ tar -xzf dosyaadi.tar.gz
   # gzip kullanılarak dosya çıkartılır.
```

```bash
$ tar -cjf dosyaadi.tar.bz2 dosya
   # dosyaadi.tar.bz2 şeklinde bzip2 kullanılarak dosya sıkıştırılır.
```

```bash
$ tar -xjf dosyaadi.tar.bz2
   # Bzip2 kullanılarak dosya çıkartılır.
```

```bash
$ gzip dosyaadi
   # gzip kullanılarak sıkıştırılma işlemi yapılır
```

```bash
$ gzip -d dosya.gz
   # gzip kullanılarak dosya çıkartılır.
```

```bash
$ gunzip dosya.gz
   # gzip kullanılarak dosya çıkartmak için kullanılabilecek farklı bir yöntemdir.
```