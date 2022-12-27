# RentACAr
## _Monolitik mimaride RentACar Projesi_


Monolitik mimaride başladığım araç kiralama projesinde aşağıdaki araçları ve teknolojileri kullandım.

- Java Spring Boot
- Exceptions
- Response-Request Pattern
- Ioc
- Model Mapper 
- Patter Design
- PostgreSQL
- Domain Driver Design

## _Entities Layer_
Veritabanı nesnelerinin tutulduğu kısımdır.

> Model,marka ve arabaya ait özellikleri  ve 
> aralarındaki ilişkileri burada tanımlarız.
>


- @OneToMany ilişkisi Model ve brand ilişkilendirilmesinde kullanıldı. 
- @OneToMany ilişkisi Car ve  model ilişkilendirilmesinde kullanıldı
- @ManyToOne ilişkisi brand ve model ilişkilendirilmesinde kullanıldı
- @ManyToOne ilişkisi model ve car ilişkilendirilmesinde kullanıldı 

## _DataAccess Layer_
Veritabanı bağlantımızı burada gerçekleştirdim.
> JpaRepository kullanıldı

## _Business Layer_
iş kodlarının yazıldığı katmandır 
>Request-Response pattern kullanıldı.Business rules , clean code, Domain Driver Design yaklaşımına uygun geliştirdim.

## _Core Layer_ 
Projeden bağımsız açık kaynak kodlarının proje içerisinde kullanılması için oluşturulan katmandır.

>Exceptions , mapping , result gibi teknikleri içerir.

## _WebApi Layer_ 
Projeyi istemci tarafına aktarmak için kullanılan katmandır.

>Bu katmanda Restful altyapısını kullandım. 


## _Application_ 

> Application dosyamızda Global Hata Yönetimi kontrolü sağlandı.
</br>
<img src= "https://github.com/berna-ozgen/rentACarProject/blob/main/src/main/java/kodlamaio/com/rentACar/ValidationException.jpg " />
</br>

> Business rules için Global Hata Yönetimi kontrolü sağlandı.
</br>
<img src= "https://github.com/berna-ozgen/rentACarProject/blob/main/src/main/java/kodlamaio/com/rentACar/BusinessExceptions.jpg" />
</br>

> Veritabanı hataları için Global Hata Yönetimi kontrolü sağlandı.
</br>
<img src= "https://github.com/berna-ozgen/rentACarProject/blob/main/src/main/java/kodlamaio/com/rentACar/DataException.jpg " />


