---
layout: post
title: Synergy &#304;le Uzaktan Bilgisayar Y&#246;netme
date: 2010-03-27 18:13
comments: true
categories: []
---
<img class="alignleft size-full wp-image-1721" title="synergy-logo" src="http://onurbaykal.com.tr/wp-content/uploads/2010/03/logo.gif" alt="" width="216" height="77" />Dizüstü bilgisayarımı bağlayabileceğim herhangi bir monitörüm yok. Ancak iki tane dizüstü bilgisayarım var ve bunları bir arada kullanmak çok verimli olurdu doğrusu. Bu düşünceden yola çıkarak - hadi gerçeği açıklayayım. Mass Effect 2'yi yatarak oynayabilmek için gidip kablosuz klavye almak yerine diğer dizüstü bilgisayarımı kablosuz klavye olarak kullanmaya çalıştım. Google'da yaptığım kısa bir aramadan sonra yanılmıyorsam 5. sonuçta aradığımı buldum. Synergy. O kadar hoşuma gitti ki bahsetmeye karar verdim. Neredeyse monitör bağlamış gibi kullanıyorum bilgisayarlarımı ve aralarında hiçbir fiziksel bağ yok. Mükemmel. Synergy birden fazla platform destekliyor. Linux kurulu laptopunuzu Windows kurulu masaüstü bilgisayarınızı kontrol etmek için kullanabilirsiniz. Bu programı sadece klavye ve fare özellikleri olan bir uzaktan bağlantı gibi düşünün.

Programın özelliklerini anlatmak kolay olmadığı gibi programı kullanmak da pek kolay değil. Neredeyse 15 dakika boyunca programın nasıl işlediğini anlamaya çalıştım. Bağlantıyı sağlamak her ne kadar kolay olmadıysa da başarılı olduktan sonra da inanılmaz derecede başarılı bir kullanım sundu. Programı tanıttıktan sonra ve deneyimlerimi anlattıktan sonra programın nasıl kullanıldığını da anlatmam gerektiğini hissediyorum. Tabii onun için yazının devamında görüşelim.<!--more-->Öncelikle buradan Synergy'nin son sürümünü indiriyoruz. Son sürüm dediğime bakmayın 2006'dan beri yeni sürüm çıkmamış ama program Windows 7'de çalışıyor.

Anlatımı kolaylaştırmak adına bir masaüstü bilgisayarı bir dizüstü bilgisayardan kontrol etmeye çalışacağız. Alınan ekran görüntüleri Windows 7 kullanan iki bilgisayardan alındı.

Öncelikle masaüstü bilgisayarımızda aşağıdaki ayarı yapıyoruz:

<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı4.png"><img class="aligncenter size-medium wp-image-1722" title="Ekran Alıntısı4" src="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı4-300x230.png" alt="" width="300" height="230" /></a>Masaüstü için client kısmını seçtikten sonra "Other Computer's Host Name" kısmına laptopun ağ içindeki yerel IP adresini yazıyoruz. Kablolu veya kablosuz ağlarda "Ağ Bağlantısı" penceresinden "Ayrıntılar" sekmesinden (Windows XP'de sekme, Windows 7 ve Vista'da bir buton) yerel IP adresini görebilirsiniz. 192.168 ile başlar bu adres.

Yukarıdaki işlemleri yaptıktan sonra "Advanced..." butonuna tıklayıp aşağıdaki pencerede çalışmaya başlıyoruz:

<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı.3PNG.png"><img class="aligncenter size-medium wp-image-1723" title="Ekran Alıntısı.3PNG" src="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı.3PNG-300x282.png" alt="" width="300" height="282" /></a>"Screen Name" kısmına çok uzun olmayan bir isim girin. Bu ismi daha sonra laptopta da kullanacağız. Tamam deyip çıktıktan sonra "Start" tuşuna basarak masaüstü bilgisayarında işlerimizi tamamlıyoruz. Bundan sonra yapacağımız işlemler dizüstü bilgisayarında (yani uzaktan yönetim işlemini gerçekleştireceğimiz bilgisayarda) yapacağız.

<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı.png"><img class="aligncenter size-medium wp-image-1724" title="Ekran Alıntısı" src="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı-300x230.png" alt="" width="300" height="230" /></a>"Server" kısmını seçiyoruz. "Configure..." butonuna bastıktan sonra aşağıdaki ekran geliyor. Bu ekran programın en önemli kısmı.

<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı1.png"><img class="aligncenter size-medium wp-image-1725" title="Ekran Alıntısı1" src="http://onurbaykal.com.tr/wp-content/uploads/2010/03/Ekran-Alıntısı1-300x208.png" alt="" width="300" height="208" /></a>Screens kısmındaki +  tuşuna basıyoruz. Masaüstü bilgisayarında verdiğimiz "Screen Name"i buraya giriyoruz. Daha sonra bir ekran daha ekliyoruz. Bu ekrana verdiğimiz ismi masaüstü bilgisayarında yaptığımız gibi bir üst pencereden "Advanced..." kısmında "Screen Name" olarak yazıyoruz.

Yaptığımız bu işlemi kısaca anlatmam gerekirse iki ekran tanımlamış oluyoruz. Alıcı ve verici. Bu senaryoda alıcı masaüstü bilgisayar, verici dizüstü bilgisayar. Alıcıda kurulu olan programda alıcının ekran ismi kayıtlı oluyor, vericide de aynı şekilde kendi ekranının ismi. Böylece program hangi ekranın hangi bilgisayara ait olduğunu anlamış oluyor. Fakat bu yeterli değil. Fareyi bir monitörden diğerine geçirmemiz lazım.

<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/03/links.png"><img class="aligncenter size-medium wp-image-1726" title="links" src="http://onurbaykal.com.tr/wp-content/uploads/2010/03/links-300x101.png" alt="" width="300" height="101" /></a>Klasik olarak bir monitörün solundan diğer monitörün sağına geçilir. Yukarıdaki ekranda bu tanım yapılı (theaob99 dizüstü, onur masaüstü . bu ayara göre dizüstünde ekranın soluna gittiğimde dizüstünün klavyesi ve faresi, masaüstünün klavyesi ve faresi olarak hareket etmeye başlayacak). İlk seçim kısmından yön, ikinci kısımda aktif ekran üçüncü kısımda ise gidilecek olan monitör oluyor. Laptoptan masaüstüne gittiniz ama masaüstünden de laptopa dönebilmelisiniz. Bu ayarı yapmayı unutmayın. Unutursanız dizüstüne geri dönemezsiniz. Bunun çözümü de masaüstünde Synergy'i kapatmak.

İşlemleri tamamladıktan sonra dizüstü bilgisayarında da Start butonuna bastığınızda bilgisayarlar bağlanmış oluyor. Tabii bu işlemin gerçekleşebilmesi için iki bilgisayar arasında aktif bir ağ bağlantısı olmak zorunda. Programla ilgili herhangi bir sorun yaşarsanız önce <a href="http://synergy2.sourceforge.net/">buraya</a> bakın. Eğer orada çözüm bulamadıysanız benimle iletişime geçerek benden yardım da isteyebilirsiniz.

Söyleyecek iki şeyim kaldı. İkisi de konuyla alakasız. İlki, şu an çok pahalı bir kablosuz klavye ve fare kullandığım. İkincisi de sinerji yaratalım mümkünse olacaktı.
