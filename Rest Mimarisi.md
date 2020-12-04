# Restful servisler nasıl çalışır? Alternatifleri nelerdir ve nasıl çalışırlar?

REST istemci-sunucu arasında hızlı ve kolay şekilde iletişim kurulmasını sağlayan bir servis yapısıdır. Açılımı Representational State Transfer olan bu ifadeyi Türkçe’ye Temsili Durum Transferi diye çevirebiliriz. REST, servis yönelimli mimari üzerine oluşturulan yazılımlarda kullanılan bir veri transfer yöntemidir. 

Burada servis yönelimli mimariyi de tanımlamak gerek. Servis yönelimli mimari  birbirinden farklı servislerin birleşip belirli yapılar oluşturarak uyumlu çalışmasını sağlayan bir yaklaşımdır. Yani servis içinde servistir. Farklı bir tanım vermek gerekirse birden fazla uygulamanın kendi içindeki modüllerinin/fonksiyonlarının başka uygulamalar tarafından kullanılabilecek şekilde tasarlandığı bir yaklaşımdır.

Rest servislerin çalışma şekline gelecek olursak eğer, Rest servisler HTTP üzerinde çalışır ve diğer alternatiflere göre daha basittir, minimum içerikle veri alıp gönderdiği için de daha hızlıdır. İstemci ve sunucu arasında XML veya JSON verilerini taşıyarak uygulamaların haberleşmesini sağlar. REST standartlarına uygun yazılan web servislerine  RESTful servisler denir. 



##  Alternatifleri

### ***1.***Falcor

Falcor modeli Netflix tarafından geliştirilen bir JavaScript kütüphanesidir. Tüm uzak veri kaynaklarının sanal bir JSON graph aracılığıyla tek bir domian model aracılığıyla temsil edilmesini sağlar. Veri toplamak için hala REST yapısını kullanır. Yani, bir request için farklı endpoint'lere istek gönderilir ve her resource için JSON object döndürülür.

### ***2.***GraphQL

GraphQL katmanı bir veya birden fazla veri kaynağı ile istemcinin arasında bulunur.İstemciden gelen istekleri alır ve gereken verileri döner. Temelde GraphQL , istemcinin istediği verilerin belirtilmesini sağlar, birden fazla kaynağın veriye ulaşılmasını kolaylaştırır ve bir tür sistem ile veriyi açıklar. yani GraphQL veri sorgulama yoğunluğuna bağlı olarak, klasik REST mimarisi ile yaşanan sorunlara istinaden (resourch yerine) oraya çıkan yeni bir yaklaşım (Application Level Query Language) olarak nitelendirilebilir.

### ***3.*** OData

OData, verileri sorgulamak ve güncellemek için REST tabanlı bir protokoldür. HTTP, ATOM /XML ve JSON gibi teknolojiler üzerine kuruludur.Yapısal olarak istemciden gönderilen sorgu isteği, sunucu tarafında işlenerek sonuç üretilmekte ve clienta gönderilmektedir. Ayrıca istemci tarafından talep edilen metadata belgesi ile OData kullandığı entitylerin detaylarından istemciyi bilgilendirebilmektedir.

