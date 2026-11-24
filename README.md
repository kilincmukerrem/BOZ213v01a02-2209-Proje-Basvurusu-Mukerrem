# BOZ213v01a02-2209-Proje-Basvurusu-Mukerrem
# Açık Uçlu El Yazısı Sınav Kâğıtlarının Görüntü İşleme ve Yerel Yapay Zekâ Destekli Rubrikle Değerlendirilmesi: Python Laboratuvarı Pilot Uygulaması


🎥 **Tanıtım videosu:** [(https://youtu.be/vCrxuONgG9o?si=YVEzOyrZy0AEwXps)]

## Videoda Anlatılanlar

Nesne tabanlı programlama derslerinde öğrenciler kodlarını ve laboratuvar
yanıtlarını deftere veya kâğıda el yazısıyla yazmaktadır. Bu kâğıtların
okunması, kodun çalıştırılıp kontrol edilmesi ve puanlanması öğretim elemanı
için zaman alıcıdır. Projenin amacı, bu aşamada öğretim elemanının işini
kolaylaştıran, bağlamı anlayan bir prototip geliştirmek ve pilot olarak
değerlendirmektir. Pilot uygulama bir Python laboratuvarı üzerinde yürütülecektir.

Önerilen sistem, el yazısı kodu görüntüden metne aktarır, kodu arka planda
güvenli biçimde çalıştırarak çıktısını denetler ve öğretim elemanının rubriğine
göre puan önerisi üretir. Proje sonunda tüm bileşenler yerelde çalışacağı için
öğrenci verisi dış servislere gönderilmeyecektir. Üretilen puan nihai karar
değildir; son kararı öğretim elemanı verir.

Videoda, proje öncesinde geliştirilen ön prototip gösterilmiştir. Bu sürüm bulut
tabanlı bir API kullanmaktadır; proje kapsamında yerel görüntü ön işleme, yerel
OCR ve yerel yapay zekâ modeliyle genişletilecektir.

Yaklaşık 50 el yazısı kâğıt üzerinde pilot çalışma yapılacaktır:

- Yaklaşık 30 kâğıdın metin karşılığı araştırmacı tarafından txt dosyası olarak girilecek; sistemin okuduğu metin bu referansla karşılaştırılarak metin tanıma başarısı karakter ve kelime hata oranlarıyla (CER ve WER) ölçülecektir.
- Sistemin verdiği puan, uzman puanlarıyla ortalama mutlak hata (MAE) ile karşılaştırılacaktır.
- Uzmanlar arasındaki uyum, sınıf içi korelasyon katsayısı (ICC) ile incelenecektir.
- Yaklaşık 10 kâğıt ikinci bir kişi tarafından da bağımsız olarak metne aktarılacak; iki insan arasındaki hata oranı, modelin hatasını yorumlamak için "insan toleransı" referansı olarak kullanılacaktır. Bu düzey geçme/kalma eşiği değildir.

Çalışma dört iş paketinden oluşmakta ve altı ay sürmektedir. Hedef, öğretim
elemanının yükünü azaltan ve veri gizliliğini koruyan bir araç ortaya koymaktır.

## Proje Akışı

Görüntü → Ön işleme → OCR / VLM → Kod çalıştırma → Rubrik puanı → Öğretim elemanı onayı

## Notlar

- Çalışma pilot niteliğindedir; bulgular genellenmeyecektir.
- Gerçek öğrenci verisi bu depoda paylaşılmamaktadır.
