Kütüphane Yönetim Sistemi

1. Projenin Amacı

Bu projenin amacı, bir kütüphanedeki kitapların, üyelerin ve ödünç alma-iade işlemlerinin ilişkisel bir veritabanı kullanılarak yönetilmesini sağlamaktır.

2. Proje Kapsamı

* Kitap bilgilerini kaydetmek ve listelemek
* Kütüphane üyelerini kaydetmek
* Kitap ödünç alma işlemlerini takip etmek
* Kitapların iade tarihlerini kaydetmek
* Ödünç alınan ve iade edilen kitapları takip etmek

3. Gereksinimler

* Her kitabın bir kitap numarası, adı, yazarı ve yayın yılı bulunmalıdır.
* Her üyenin bir üye numarası, adı, soyadı ve iletişim bilgisi bulunmalıdır.
* Bir üye birden fazla kitap ödünç alabilmelidir.
* Her ödünç alma işlemi için ödünç alma tarihi, iade tarihi ve iade durumu kaydedilmelidir.
* Kitaplar, üyeler ve ödünç alma işlemleri arasında ilişkiler kurulmalıdır.

4. Planlanan Veritabanı Tabloları

* Kitaplar
* Üyeler
* Ödünç İşlemleri

5. Kullanılacak Araçlar

* GitHub
* Mermaid veya draw.io (ER diyagramı için)
* İlişkisel veritabanı tasarım ilkeleri

6. İş Kuralları

* Her kitabın benzersiz bir KitapID değeri olmalıdır.
* Her üyenin benzersiz bir UyeID değeri olmalıdır.
* Her ödünç alma işlemi yalnızca bir üyeye ve bir kitaba bağlı olmalıdır.
* Bir üye, farklı zamanlarda birden fazla ödünç alma işlemi gerçekleştirebilir.
* Bir kitap, farklı zamanlarda farklı ödünç alma işlemlerinde yer alabilir.
* İade işlemi gerçekleştiğinde iade durumu güncellenmelidir.

7. Varlıklar ve İlişkiler

* Kitaplar: Kitap bilgilerini tutar.
* Üyeler: Kütüphane üyelerinin bilgilerini tutar.
* Ödünç İşlemleri: Kitapların kim tarafından ve ne zaman ödünç alındığını tutar.
* Üyeler – Ödünç İşlemleri: Bire çok (1:N) ilişki.
* Kitaplar – Ödünç İşlemleri: Bire çok (1:N) ilişki.

8. ER Diyagramı

Projenin veritabanı tasarımını gösteren ER diyagramı aşağıdaki dosyada bulunmaktadır.

[ER Diyagramını Görüntüle](kutuphane-er-diyagrami.drawio.png)
