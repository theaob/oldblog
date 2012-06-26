---
layout: post
title: jList&#039;e DefaultListModel ile Yeni &#214;ge Ekleme
date: 2009-10-04 22:34
comments: true
categories: []
---
<img class="alignleft size-full wp-image-1377" title="events_468" src="http://onurbaykal.com.tr/wp-content/uploads/2009/10/events_468.jpg" alt="events_468" width="200" height="160" />Tobb Etü'de yeni bir dönem başladı. Hatta başlayalı baya oldu. 5. haftaya girdik. 6. hafta (gelecek hafta) vizeler başlıyor ve kimi üniversiteler daha eğitime başlamadı. Çalışıyoruz gördüğünüz gibi. Bu dönem Bil211 kodlu dersi alıyorum. Nesnesel Tasarım ve Programlama (yabancı dilde eğitim alanlar için Object Oriented Design &amp; Programming) yani. Geçen sene 2. dönem (bizim okul 3 dönem, 2. sınıftan itibaren bir dönem staja gönderiyor) Java'ya temel bir giriş yapmıştık. Fakat GUI namına bir şey görmemiştik. Bu derste ise nesnesel programlanın inceliklerini öğreniyoruz. Hocamız da ödev olarak GUI'li bir program verdi. Açıkçası kimileri tartışabilir öğretmediği şeyi istiyor diye, açık konuşmak gerekirse başta bende böyle düşünüyordum ama bu lafı söyleyenin ödevi yapmaya başlamayan birinin olduğunu anladım. İnternet gerçekten bir deniz, aradığınız her şeyi buluyorsunuz. İş gerçekten sizin ne kadar bilgiye aç olduğunuza bakıyor. Uzun lafın kısası ödev <a href="http://mkgungor.googlepages.com/homework133">bu</a> (adres sonradan değişebilir belki). Basit bir program aslında. Fakat yeni şeyler öğrenmek gerektiriyor. Bu yüzden hafif bir zorluğu var.

Netbeans ile hem GUI hem de programlamayı yaptım. Hafifçe hem yaptığım işlemin mantığını anlatayım hem de kod örneği vereyim. Öncelikle jList'i Properties'den Custom Code haline getirip DefaultListModel olarak tanımladığım nesneyi veriyorum.
<pre lang="java">
//DefaultListModel kullanabilmek için aşağıdaki paketi import etmek gerekiyor
import javax.swing.DefaultListModel;

//model nesnesini kodun başlarında tanımladım
DefaultListModel model = new DefaultListModel();

//i Index'li bir nesneyi jList'ten kaldırmak için böyle bir kod yazıyoruz:
model.remove(i);

//Listeyi baştan sıralamak için veya tüm elemanları silmek için:
model.removeAllElements();

//Aşağıdaki kod ile listenize yeni bir nesne ekleyebilirsiniz
model.addElement(Object o);
//Bu listeye sondan ekler ama dikkat edin listeyi yeniden sıralıyorsanız, en üste de getirebilirsiniz.
</pre>
