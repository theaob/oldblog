---
layout: post
title: Yine Yeniden YouTube Engeli
date: 2010-06-02 15:11
comments: true
categories: []
---
<a href="http://onurbaykal.com.tr/wp-content/uploads/2010/06/logo_masthead.png"><img class="alignleft size-full wp-image-1804" title="logo_masthead" src="http://onurbaykal.com.tr/wp-content/uploads/2010/06/logo_masthead.png" alt="" width="98" height="39" /></a>Gazze'ye yardım giremiyor, bizim ülkeye de YouTube. Yine ayarlarla oynamışlar. YouTube'u kapatalım derken Google Docs, Google Charts ve Google Analytics de patlamış. Bravo valla. İşleri güçleri yok bizim kötü şeyler görmememiz için uğraşıyorlar. Neyse şimdilik bu çözümü uygulayın, daha işe yarar bir şey bulursam tekrar yazarım.

Windows kurduğunuz dizin altında Windows\System32\Drivers\etc\ konumuna kadar geliyorsunuz. Buradaki hosts dosyasını not defteriyle açıyoruz ve aşağıdaki satırları ekliyoruz:

209.85.229.99 www.youtube.com
209.85.229.99 youtube.com

Daha sonra DNS ayarlarımızı da 8.8.8.8 ve 8.8.4.4'e geri getiriyoruz. Böylece YouTube'a girilebiliyor ama diğer Google servislerinde hala problemler var.
