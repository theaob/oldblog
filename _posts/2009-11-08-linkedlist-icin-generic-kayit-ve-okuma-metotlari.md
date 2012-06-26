---
layout: post
title: LinkedList i&ccedil;in Generic Kay&#305;t ve Okuma Metotlar&#305;
date: 2009-11-08 09:27
comments: true
categories: []
---
Bil 211 dersinin ödevlerinde sıkça dosya kaydetme ve dosya okuma işlemlerinin kullanılması gerekiyordu. 3 class için 3 farklı LinkedList olduğundan (koddaki LinkedListler ArrayList ile değiştirilirse de çalışır) 3 kere de ayrı ayrı kaydetme ve okuma metotları yazmıştım. İkinci ödevi yaparken aklımdan ortak bir kod yazmayı geçirdim ancak nasıl üstesinden geleceğim konusunda bir çözüm bulamamıştım. Enes ile proje için kod yazarken ortak bir dosya kayıt ve dosya okuma metodu fikrimi söyleyince generic olarak bir metot yazılabileceğini önerdi. O gün birlikte de buna benzer bir class yazdık, tabii o kodun üstüne farklı geliştirmeler yapıldı. O yüzden ben ayrı olarak hem ödevlerde hem de projede kullanılabilecek bir class örneği hazırladım. Sabahın köründe hazırladığım için kodumdan pek memnun değilim ancak yine de gerekli işlevi görecektir.
<pre lang="java">
import java.io.FileInputStream;
import java.io.FileOutputStream;
import java.io.ObjectInputStream;
import java.io.ObjectOutputStream;
import java.util.LinkedList;

/**
 * @author Onur Baykal
 */
public class DosyaIslemleri {
    /**
     *
     * @param &lt;E&gt; LinkedList türü
     * @param liste Kaydedilmek istenen LinkedList list, türü önemli değil
     * @param dosyaAdi Kaydedilecek olan dosyanın adı
     */
    public &lt;E&gt; void listeKaydet(LinkedList&lt;E&gt; liste, String dosyaAdi){
        try{
            FileOutputStream fos = new FileOutputStream(dosyaAdi);
            ObjectOutputStream oos = new ObjectOutputStream(fos);
            oos.writeObject(liste);
            oos.close();
            fos.close();
        }catch(Exception e){

        }
    }
     /**
     * Bu method daha önce yaratılmış bir LinkedList'in içinin doldurulmasına
     * yarar. Yüklenecek olan listenin türünü belirlemek için parametre olarak
     * liste alır.
     * @param &lt;E&gt; LinkedList türü
     * @param liste Üzerine yükleme yapılacak olan liste,
     * @param dosyaAdi İçerisinden liste yüklecek olan dosyanın adı
     * @return Üzerine kayıtlı olan liste yüklenmiş olan liste geri döndürülür
     */
    public &lt;E&gt; LinkedList&lt;E&gt; listeYukle(LinkedList&lt;E&gt; liste,String dosyaAdi){
        try{
            FileInputStream fis = new FileInputStream(dosyaAdi);
            ObjectInputStream ois = new ObjectInputStream(fis);
            liste = (LinkedList&lt;E&gt;)ois.readObject();
            ois.close();
            fis.close();
        }catch(Exception e){

        }
        return liste;
    }
}</pre>
