# Sharpe-oranı-hesaplayıcı-

Sharpe Oranı Hesaplayıcı (C Dili):

Bu C programı, yatırım portföylerinin alınan riske göre getiri fazlalığını ölçen Sharpe Oranını kullanıcıdan alınan girdilerle hesaplar ve sonucu yorumlar. Program, girdi hatalarına karşı güvenilir olacak şekilde tasarlanmıştır.

Programın Amacı:

Ana amaç, bir finansal enstrümanın (portföy, hisse senedi, fon vb.) performansını, risksiz bir yatırım aracına kıyasla ne kadar iyi olduğunu nicel olarak değerlendirmektir. Yüksek Sharpe oranı, yatırımın risk birimi başına daha iyi getiri sağladığı anlamına gelir.

Özellikler:

-Güvenilir Girdi (Input Handling): scanf fonksiyonu ile sayısal girdi beklenirken kullanıcı metin veya geçersiz karakter girdiğinde programın çökmesi yerine, kullanıcıya hata mesajı göstererek kontrollü bir şekilde sonlanır.

-Girdi Arabelleği Temizleme: clearInputBuffer() özel fonksiyonu kullanılarak, scanf sonrası girdi arabelleğinde kalan artçı karakterlerin (\n gibi) bir sonraki girdiyi bozması engellenir.

-Standart Sapma Doğrulama: Hesaplama hatasını önlemek için standart sapmanın sıfır veya negatif olup olmadığı kontrol edilir.

-Yorumlama: Hesaplanan Sharpe oranına göre (Negatif, 0, Düşük, İyi, Çok İyi, Mükemmel) yorumsal bir değerlendirme sunar.

-Hassasiyet Kontrolü: Sonuç, %.2f formatı kullanılarak iki ondalık basamak hassasiyetle gösterilir.

Hesaplama Formülü:

$$\text{Sharpe Oranı} = \frac{\text{Yatırım Getirisi} - \text{Risksiz Faiz Oranı}}{\text{Portföyün Standart Sapması}}$$

Kullanım ve Örnek Çıktı:

Girdi Parametresi,Kullanıcı Girdisi

Yatırım Getirisi,18.0

Risksiz Faiz Oranı,4.0

Standart Sapma,7.0

$$\text{Sharpe Oranı} = \frac{18.0 - 4.0}{7.0} \approx 2.00$$

Çıktı:

=== Sharpe Orani Hesaplayici ===

Yatirim getirisi (% cinsinden): 18.0

Risksiz faiz orani (% cinsinden): 4.0

Portfoyun standart sapmasi (% cinsinden): 7.0


Sharpe Orani = 2.00

-> Sharpe orani 2.00: Cok iyi bir performans.Iyi gunler dileriz!

Hata Kontrolü Örneği:

 Kullanıcının sayı yerine harf girdiği bir senaryo:

 === Sharpe Orani Hesaplayici ===
 
Yatirim getirisi (% cinsinden): ABC

Gecersiz giris! Lutfen sayi giriniz.

(Program bu noktada güvenli bir şekilde sonlanır.)



