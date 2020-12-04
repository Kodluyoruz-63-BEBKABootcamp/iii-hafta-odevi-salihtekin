# ViewData, ViewBag, TempData farkları nelerdir?

***ViewBag***, nesnesi Run Time’da oluşan ve verileri controller'dan view'e geçirmek için kullanılan dinamik bir nesnedir. Kullanımı;

`ViewBag.ad = "salih tekin";`

***ViewData***, ViewDataDictionary sınıfı ile Key/Value ilişkisine göre çalışır.ViewBag ile benzer işleve sahiptir. Kullanımı;

`ViewData["ad"]= "salih tekin";`

***TempData***, diğer iki nesne ile aynı kullanım amacına sahip taşıma nesnesidir. Kullanımı;

`TempData["ad"]= "salih tekin";`

Bu üç nesnenin farkına bakacak olursak eğer;

Öncelikle ViewBag nesnesinin dinamik tipte bir nesne olduğunu belirtmiştik. Bundan dolayı, ortaya çıkabilecek hatalar derleme zamanında (Compile Time) değil çalışma zamanında (Run time) yakalanacaktır. Bunun dışında ViewData ile bir farkı bulunmamaktadır. TempData nesnesi ise diğer ikisine nazaran büyük bir farklılığa sahiptir. Diğer iki nesne anlık HTTP istek içerisinde geçerlidir. Bir sonraki istekte geçerliliklerini yitirir. Fakat TempData nesnesi, o anki HTTP isetik tarafından üretilip bir ve birden fazla view üzerinde kullanılabilir.  