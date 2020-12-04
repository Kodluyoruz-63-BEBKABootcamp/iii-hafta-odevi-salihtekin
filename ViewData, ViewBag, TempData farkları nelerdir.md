# ViewData, ViewBag, TempData farkları nelerdir?

***ViewBag***, nesnesi Run Time’da oluşan ve verileri controller'dan view'e geçirmek için kullanılan dinamik bir nesnedir. Kullanımı;

```c#
ViewBag.Ad = "Salih Tekin";
```

***ViewData***, ViewDataDictionary sınıfı ile Key/Value ilişkisine göre çalışır.ViewBag ile benzer işleve sahiptir. Kullanımı;

```c#
ViewData["Ad"] = "Salih Tekin";
```

***TempData***, diğer iki nesne ile aynı kullanım amacına sahip taşıma nesnesidir. Kullanımı;

```c#
TempData["Ad"] = "salih tekin";
```

Bu üç nesnenin farkına bakacak olursak eğer;

Öncelikle ViewBag nesnesinin dinamik tipte bir nesne olduğunu belirtmiştik. Bundan dolayı, ortaya çıkabilecek hatalar derleme zamanında (Compile Time) değil çalışma zamanında (Run time) yakalanacaktır. Bunun dışında ViewData ile bir farkı bulunmamaktadır. TempData nesnesi ise diğer ikisine nazaran büyük bir farklılığa sahiptir. Diğer iki nesne anlık HTTP istek içerisinde geçerlidir. Bir sonraki istekte geçerliliklerini yitirir. Fakat TempData nesnesi, o anki HTTP isetik tarafından üretilip bir ve birden fazla view üzerinde kullanılabilir.  