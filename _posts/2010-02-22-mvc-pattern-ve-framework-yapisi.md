---
layout: post
title: MVC Pattern ve Framework Yap&#305;s&#305;
date: 2010-02-22 19:05
comments: true
categories: []
---
Herhangi bir proje sıfırdan geliştirileceği zaman genellikle nereden başlanacağı doğru belirlenmez. Bunun nedeni kodlama işlemi esnasında hangi pattern (desen, örüntü) kullanılacağı bilinmediğindendir. Birden fazla kişinin üzerinde çalıştığı projelerde bu sorun (bence) daha belirgindir. Eleman başına düşen kısımın nasıl geliştirileceği (belirtilmediyse) tamamen geliştiriciye bağlıdır. Bu ve bunun gibi sorunlar yaşamamak için biz bilgisayar mühendislerine belirli patternler öğretilir. Öğrenirken pek anlaşılır ve mantıklı gelmese de uygulaması bunun tamamen zıttıdır. Pek çok işlemi kolaylaştırmak için sıkça patternler ve frameworkler kullanılır. Öncelikle framework nedir bundan bahsedeyim daha sonra da MVC'ye ucundan dokunayım.

Framework çeviri olarak çatı veya çerçeve olarak kullanılsa da bence tam olarak anlamını karşılamıyor. Terim olarak belirli bir pattern üzerine kurulmuş, belirli temel kodlamaları yapılmış ve geliştiricinin bazı yaygın fonksiyonları kolayca kullanmasını sağlayan yapılardır. Çoğunlukla MVC (Model-View-Controller) Pattern üzerine kurulmuş Frameworkler popüler ve kullanım olarak kolaydır. Web tabanlı projeler için daha uygun olmasına rağmen masaüstü yazılımları için de kullanılabilecek olan Frameworkler var. Ben MVC Pattern ile <a href="http://cakephp.org">CakePHP</a> ile tanıştım. Açıkçası öğrenme aşaması hem kolay oldu hem de mantığı çok iyi kavrattı.
<h2>Model-View-Controller Pattern</h2>
<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/02/mvc-php.png"><img class="alignleft size-medium wp-image-1685" title="mvc-php" src="http://onurbaykal.com.tr/wp-content/uploads/2010/02/mvc-php-300x283.png" alt="" width="300" height="283" /></a>MVC hayatı kolaylaştıran bir pattern. Ögelerinin baş harflerinden oluşuyor.

Model, veritabanı ile ilgili işleri hallediyor. Bu neredeyse bir scriptin veritabanı ayarlarını ayarlamak kadar kolay. Veritabanı tabloları oluşturulduktan sonra Model gerekli bilgilerle dolduruluyor ve Frameworkünüz veritabanı bağlantısını otomatik olarak sağlıyor. Veritabanı doğrulamaları da buradan yapılıyor. Frameworke göre bazı değişiklikler olsa da genellikle birbirlerine benziyorlar.

View, kullanıcıya yansıtılacak olan şeylerin belirlendiği öge. Burada program kodundan çok HTML oluyor. Elbette veritabanından alınan verileri yazdırmak için kod kullanılıyor ama burada oldukça az olarak kod kullanılıyor. Kod kullanımı da oldukça sınırlı. Öntanımlı metotlar dışında dilin kendi kodları kullanılabiliyor. Frameworklerin View'da kullanılabilecek olan metotları genellikle belli ve çok daha sınırlı oluyor.

Controller, işlemlerin yapıldığı öge. Burada metotlar, View'a ne gönderileceği, veritabanı işlemleri (CRUD, create, read, delete, update) yazılıyor. Projenizin bel kemiği Controller kısmı. Geliştirme işleminin çoğu da burada  oluyor. İşlem gücü gerektiren şeyler de Controller üzerinden gerçekleştiriliyor.

Anlattıklarım pek açık gelmediyse yandaki resim biraz daha açıklayıcı olabilir. Tabii o resim PHP için (hatta internet bazlı Frameworkler için diye genelleyebiliriz) yapılmış.

<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/02/350px-ModelViewControllerDiagram.svg_.png"><img class="alignright size-medium wp-image-1686" title="350px-ModelViewControllerDiagram.svg" src="http://onurbaykal.com.tr/wp-content/uploads/2010/02/350px-ModelViewControllerDiagram.svg_-300x141.png" alt="" width="300" height="141" /></a>MVC Frameworklerinin kolaylığı, veritabanı işlemlerinin kolay olması, sık gerçekleştirilen işlemlerin metot olarak önceden tanımlanmış olması, Framework yeterli olmadığı zaman kullanılan dille eklemeler yapılabilmesi, farklı görevleri olan kodların ayrı olması ve böylece işlerin kolaylaşması, eklenti desteği, javascript, ajax kullanımının kolaylaştırılması... olarak sıralanabilir. Bahsetmediğim bir durum ise bazı MVC Frameworklerde dosya isimlerinin serbest olmaması. Örneğin <a href="http://cakephp.org">CakePHP</a>'de dosya isimleri şu şekilde: veritabanı tabloları çoğul, o tablonun Modeli tekil, Controllerı çoğul ve sonunda "_controller" etkli, Viewü ise Controllerda tanımlanan metot ismiyle aynı olmak zorunda. Karışık gelebilir ama gerçekten çok zor değil. Tabii bu her Frameworkte böyle değil.

<a href="http://cakephp.org">CakePHP</a>'den sonra <a href="http://rubyonrails.org/">Ruby on Rails</a>'i de merak ettim. Sonuçta büyük projelerde yaygın olarak kullanılan MVC Frameworkü Ruby on Rails. Twitter, Xing, Shopify, Github, Lighthouse... gibi büyük servisler Ruby on Rails ile yazılmış. Ruby on Rails, <a href="http://www.ruby-lang.org/">Ruby programlama dili</a>ni kullanıyor. Ruby insanların okuyup kodun ne yaptığını anlayabileceği dillerden biri. Gerçekten sizi kendine hayran edecek özellikleri var. Python'a oldukça benziyor. Ruby on Rails konusunda şimdilik çok fazla bir şey söyleyemiyorum çünkü ben de hala tam olarak öğrenmiş değilim. Belki gün gelir Rails ile ilgili bir yazı da yazarım.
<h2>Bazı MVC Frameworkler ve Dilleri</h2>
CakePHP - <a href="http://www.cakephp.org">http://www.cakephp.org</a> - PHP

Zend Framework - <a href="http://framework.zend.com/">http://framework.zend.com</a> - PHP

Symfony - <a href="http://www.symfony-project.org/">http://www.symfony-project.org/</a> - PHP

Ruby on Rails - <a href="http://rubyonrails.org/">http://rubyonrails.org/</a> - Ruby

Cocoon - <a href="http://cocoon.apache.org/">http://cocoon.apache.org/</a> - Java

JavascriptMVC - <a href="http://www.javascriptmvc.com/">http://www.javascriptmvc.com/</a> - JavaScript

CodeIgniter - <a href="http://codeigniter.com/">http://codeigniter.com/</a> - PHP

Django - <a href="http://www.djangoproject.com/">http://www.djangoproject.com/</a> - Python

CppCMS - <a href="http://cppcms.sourceforge.net/wikipp/en/page/main">http://cppcms.sourceforge.net/wikipp/en/page/main</a> - C++
