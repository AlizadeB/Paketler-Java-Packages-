
# Paketlər (JAVA Packages)

Java-da paket əlaqəli sinifləri qruplaşdırmaq üçün istifadə olunur. Qısaca Java paket bizim üçün bir qovluqdur. 

![Uygulama Ekran Görüntüsü](https://www.scientecheasy.com/wp-content/uploads/2020/06/java-predefined-packages.png)

## Paketlərə niyə ehtiyacımız var?

Biz ad konfliktlərinin qarşısını almaq və daha yaxşı saxlanıla bilən kod yazmaq üçün paketlərdən istifadə edirik. 

## Bu konflikt tam olaraq nə deməkdir?

Tutaq ki, bizim A və B qovluqlarımız var. Hər iki qovluqda İstifadəçilər sinfi var. Biz bu iki sinif arasındakı fərqi paketlər vasitəsilə açıqlayırıq. Bir qədər sonra bunu nümunə ilə göstərəcəyik.

Bir nüansı da qeyd edək ki paket adlarını kiçik hərflə yazmaq lazımdır ki Sinif adları böyüklə yazıldığı üçün başqa bir konflikt ortaya çıxmasın.

## Paketlər iki kateqoriyaya bölünür:
-	#### Javanın öz daxili Paketləri (Java API paketləri)
-	#### İstifadəçi tərəfindən hazırlanmış Paketlər 

### Daxili Paketlər
Java API Java İnkişaf Mühitinə daxil edilmiş, istifadəsi pulsuz olan əvvəlcədən yazılmış siniflərin kitabxanasıdır.

Bu hazır kitabxanalarda (paketlərdə) daxiletmənin idarə edilməsi, verilənlər bazası proqramlaşdırması və daha çox şey üçün komponentlər var. Tam siyahını Oracles saytında tapa bilərsiniz: https://docs.oracle.com/javase/8/docs/api/.

#### Bəs yaxşı bu daxili paketlərə nə ehtiyac var, olmazmı ki istədiyim sinfi istədiyim metodu istədiyim vaxt istifadə edim?

Təəssüflər olsun ki, kompüter dünyası hələ də bunun üçün hazır deyil. Çünki bu qədər paket eyni anda istifadə olunsa donmalar, gecikmələr baş verər. Bu səbəbdən “hazırladığınız yeməyin resseptinə uyğun qidalardan” istifadə edin.

Kitabxana paketlərə və siniflərə bölünür. Bu o deməkdir ki, siz bütöv bir paketi də o paketin sadəcə bir sinfini də çağıra bilərsiniz.  Gəlin bunu aşağıdakı nümunə üzərindən izah edək. Bunu da vurğulamaq lazımdır ki müvafiq paketi çağırmaq üçün **import** açar sözündən istifadə olunur.

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/e9b5b007808c44504ab96c4c483efc9c.png)

Buradakı nümunədə util paketinin Scanner sinfi və lang paketi bütöv şəkildə (* bütün mənasındadır) çağrılmışdır.

### Static açar sözünün paketlərdə istifadəsi

Yenə static bizim köməyimizə gəldi. Bunu nümunədə daha rahat görə bilərik:

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/0438fa6bd14c7826016f48a0d0c8c5be.png)

### Maraqlı bir problem

Problemin maraqlı olmasına səbəb Date sinfidir. Bu sinif hazır şəkildə iki paketin daxilində fərqli şəkildə mövcuddur. Biz əgər hər ikisini çağırsaq istifadə zamanı proqram xəta verəcək:

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/74678b158dbe267f3a2ea7a0163d11ac.png)

Bu konflikti aradan qaldırmaq üçün bir başa olaraq paketin vasitəsilə referans dəyişəni yaradaraq problem aradan qaldırılır:

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/bc4d4f367757ad785d32fd1a3671eba9.png)

### İstifadəçi paketləri

Bu paketlər proqramçı tərəfindən hər hansı bir layihə üçün yaradılan paketlərdir. Paket yaradarkən siz paket üçün ad seçməli və paketə daxil etmək istədiyiniz sinifləri, interfeysləri, siyahıları və annotasiya növlərini ehtiva edən hər bir mənbə faylın yuxarı hissəsində həmin adla birlikdə paket bəyanatını daxil etməlisiniz. Paket yaratmaq üçün **package** açar sözündən istifadə olunur:

![Uygulama Ekran Görüntüsü](https://i2.paste.pics/2751312cb0268bd20641ce89def0ded4.png)

`Unutmayın əgər bir tələbə sadəcə öz müəlliminin dediyi ilə kifayətlənirsə o öyrənmir sadəcə təqlid edir. Bu səbəbdən hər zaman araşdırın. İstinadları gözdən keçirin.`

## İstinadlar

Bu yazı aşağıdaki mənbələrdən yararlanılaraq hazırlanmışdır:

- https://www.geeksforgeeks.org/packages-in-java/
- https://www.w3schools.com/java/java_packages.asp
- https://www.javatpoint.com/package
- https://www.tutorialspoint.com/java/java_packages.htm
