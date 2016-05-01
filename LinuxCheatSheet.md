.____    .__                      _________ .__                   __      _________.__                   __
|    |   |__| ____  __ _____  ___ \_   ___ \|  |__   ____ _____ _/  |_   /   _____/|  |__   ____   _____/  |_
|    |   |  |/    \|  |  \  \/  / /    \  \/|  |  \_/ __ \\__  \\   __\  \_____  \ |  |  \_/ __ \_/ __ \   __\
|    |___|  |   |  \  |  />    <  \     \___|   Y  \  ___/ / __ \|  |    /        \|   Y  \  ___/\  ___/|  |
|_______ \__|___|  /____//__/\_ \  \______  /___|  /\___  >____  /__|   /_______  /|___|  /\___  >\___  >__|
        \/       \/            \/         \/     \/     \/     \/               \/      \/     \/     \/


===================================================================================================================

#===Dosya Komutları===#

$cat filename

dosya içeriğini gösterir.

---

$cat > filename

Dosyaların standart girişten listelenmesi

---

$cd

Dizini değiştirmek için kullanılan komut

---

$cmp

Herhangi iki tür dosyayı karşılaştırır ve sonucu standart çıktıya yazar. Eğer dosyalar aynıysa öntanımlı olarak cmp komutu birşey yapmaz. Eğer farklıysalar, ilk farkın oluştuğu bayt ve satır sayısı gösterilir.

---

$cp originalfilename newfilename

dosya ve dizinleri kopyalar

---

$cut

girişin herbir satırındaki bölümleri alıp ekranda gösterir

---

$diff

Bilgisayar ile hesaplamada bir dosya karşılaştırma yardımcı programıdır ve iki dosya arasındaki farkları bulmaya yarar.

---

$join

iki dosyanın satırlarını ortak bir alanda birleştirir.

---

$ls -l

dosyalar hakkında bilgi listeler

---

$ls -la

dosyalar hakkında bilgi listeler gizli dosyalarda dahil

---

$mkdir

yeni bir dizin oluşturur

---

$mv

belirtilen dosyayı yeniden adlandırır yada taşımaya yarar

---

$nl

satır sayısını gösterir.

---

$touch filename

yeni bir dosya oluşturma

---

$pwd

içinde bulunduğu dizinin ismini gösterir

---

$rm -rf dirname

dosya ve dizinleri siler

---

$wc

Kelime Sayma İşlemlerini Gerçekleştiren Komuttur

---

$ln -s filename link

sembolik link oluşturur.

---

$head

Her DOSYA'nın ilk on satırını standart çıktıya yazar.

---

$tail

Belirtilen her DOSYA'nın son 10 satırını standart çıktıya yazar.

---

$tail -f

Belirtilen her DOSYA'nın son 10 satırını sürekli izleyerek standart çıktıya yazar.

#===SSH & Güvenli Dosya İşlemleri===#

$scp dosyaadi kullaniciadi@uzaksunucu:/home/

uzak sunucuya güvenli bir şekilde dosya aktarımına yardımcı olur.

---

$sftp

Dosya transferi için alternatif bir uygulama

---

$ssh user@host

sunucuya kullanıcı adınız ile giriş yapabilirsiniz.

---

$ssh -p user@host

özel tanımlanan port numarası ile sunucuya kullanıcı adınız ile giriş yapabilirsiniz.

---

$ssh-copy-id user@host

şifre olmadan ssh key aracılığı ile giriş yapmayı etkinleştirir.

#===Süreç Yönetimi===#

$ps

Aktif olan tüm işlemleri gösterir(bash,root,su vb)

---

$top

Çalışan sistemdeki tüm işlemleri gösterir

---

$kill pid

Çalışan bir uygulamayı pid numarasına göre sonlandırır.

---

$killall proc

proc ile başlatan tüm işlemleri sonlandırır.

---

$bg

arka plandaki işlerin tamamını durdurur.

---

$renice

çalışan işlemlerin önceliğini değiştirmek için kullanılır.

#===Grup & Dosya İzinleri===#

$chmod

dosyanın iznini değiştirmeye yarar

---

$chgrp

grup-id ye göre grup izinlerini değiştirmeye yarar.

---

$groups

grup üyeliklerinde değişiklik

#===Arama Komutları===#

$grep [pattern] dosya

belirtilen pattern göre dosyalarda arama yapar.

---

$grep -r [pattern] klasör

özyenileme yöntemi ile dizin içerisinde arama yapar

---

$find dosya

dosyanın tüm örneklerini bulmaya yarar.(UNİX)

---

$locate dosya

dosyanın tüm örneklerini bulmaya yarar.

---

$xargs

argüman listesi oluşturmaya yarar.Oluşturulan bu listeye görede başka komutlar tetikler

#===Sıkıştırma Komutları===#

$tar -xf dosyaadi.tar

dosyaadi.tar içerisindeki dosyaları çıkartır

---

$tar -cf dosyaadi.tar dosyaadi

dosyaadi.tar şeklinde sıkıştırılmış dosya oluşturur.

---

$tar -czf dosyaadi.tar.gz

gzip kullanarak dosyaadi.tar.gz oluşturur.

---

$tar -xzf dosyaadi.tar.gz

gzip kullanılarak dosya çıkartılır.

---

$tar -cjf dosyaadi.tar.bz2 dosya

dosyaadi.tar.bz2 şeklinde bzip2 kullanılarak dosya sıkıştırılır.

---

$tar -xjf dosyaadi.tar.bz2

Bzip2 kullanılarak dosya çıkartılır.

---

$gzip dosyaadi

gzip kullanılarak sıkıştırılma işlemi yapılır

---

$gzip -d dosya.gz

gzip kullanılarak dosya çıkartılır.

---

$gunzip dosya.gz

gzip kullanılarak dosya çıkartmak için kullanılabilecek farklı bir yöntemdir.
