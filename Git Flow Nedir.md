# Git Flow Nedir

 Git flow git üzerindeki branching sisteminin daha düzenli olmasını sağlayan bir git eklentisidir.Git flow kullanarak projelerde oluşabilecek hataları, düzensiz çalışmayı ve benzeri durumları en aza indirmiş oluruz.Git flow kendi içinde branch'lere ayrılmaktadır.

Bunlardan biri master branch. Bu branch'in içinde temel kullandığımız kod bulunmaktadır. Bu branch en stabil şekilde çalışan branch'dir.

diğeri development branch'i bulunmaktadır.Bu master'dan aldığımız bir branch'dir.Hali hazırda geliştirdiğimiz ve gelişmekte olan kodu barındırır. Eğer yapılan kod master'a gidicekse development üzerinden master'a geçilir. Development baranch de çalışma yapmak için ise bir feature branch açılır. Bu branç hali hazırda geliştirmenin yapıldığı ve birçok kişi tarafından da açılarak yapılabileceği branch'dir. Yapılan değişimler birleştirilerek development branch'e gönderilir.

## Github flow vs Git flow

Yukarıda git flowdan bahsettik. Github flow ise git flowun basitleştirilmiş halidir.Git flowda oluşturulan dallanmalara bazen ihtiyaç duyulmayabilir. Github flow bu durumu ortadan kaldırmak için iki dallanmalı seürekli gelişimli bir yapı oluşturmuştur. İlk dallanma master ikinci dallanma ise geliştirme ortamının olduğu dallanmadır iş akışı bu iki dal üzerinden ilerlemektedir.