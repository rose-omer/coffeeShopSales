# Coffee Sales Data Analysis

## Proje Tanıtımı

Bu proje, **Kaggle**'da yer alan **Coffee Sales** veri setini kullanarak bir dizi veri analizi işlemi yapmayı amaçlamaktadır. Veri seti, bir kahve dükkanının satış işlemleri hakkında çeşitli bilgiler içermektedir. Bu analizde, satış miktarı, ürün fiyatı ve toplam işlem değeri gibi sayısal veriler ile kategorik veriler kullanılarak çeşitli görselleştirmeler yapılmıştır.

Veri seti, satışların ve ürünlerin özelliklerini içeren aşağıdaki sütunlardan oluşmaktadır:
- **transaction_id**: Her bir satış işleminin benzersiz kimliği.
- **transaction_date**: Satışın gerçekleştiği tarih.
- **transaction_time**: Satışın gerçekleştiği saat ve dakika.
- **transaction_qty**: Satılan ürün miktarı.
- **store_id**: Satışın yapıldığı dükkanın kimliği.
- **store_location**: Dükkanın konumu.
- **product_id**: Ürünün kimliği.
- **unit_price**: Ürünün birim fiyatı.
- **product_category**: Ürünün kategorisi (örneğin, Kahve, Çay, Fırın).
- **product_type**: Ürünün türü (örneğin, Espresso, Scone, vb.).
- **product_detail**: Ürünün ayrıntıları.

Bu analizde, veri setindeki sayısal değişkenlerin (satış miktarı, birim fiyatı ve toplam işlem değeri) ve kategorik değişkenlerin dağılımı ve ilişkileri incelenmiştir.

## Veri Kaynağı

Veri seti, Kaggle üzerinden elde edilmiştir. İlgili kaynak: [Coffee Sales Data on Kaggle](https://www.kaggle.com/datasets/ahmedabbas757/coffee-sales/data)

## Kullanılan Teknolojiler

- **Python**: Veri analizi için kullanılan ana programlama dili.
- **Pandas**: Veri işleme ve analiz için.
- **Matplotlib** ve **Seaborn**: Veri görselleştirmeleri için.
- **Jupyter Notebook**: Analizlerin yapıldığı ortam.

## Yöntem

1. **Veri Yükleme**:
   - İlk olarak, veri seti CSV formatında Pandas kullanılarak yüklendi.
   
2. **Veri Temizliği ve Ön İşleme**:
   - Eksik değerler kontrol edilip temizlendi.
   - Veri türleri doğru şekilde ayarlandı.
   - `total_transaction_value` (toplam işlem değeri) yeni bir sütun olarak hesaplandı, bu sütun satış miktarının birim fiyatla çarpılmasıyla oluşturuldu.

3. **Veri Analizi**:
   - **Deskriptif İstatistikler**: Veri setindeki sayısal değişkenlerin temel istatistikleri çıkarıldı.
   - **Korelasyon Analizi**: Sayısal değişkenler arasındaki ilişkiler incelendi ve korelasyon matrisi oluşturuldu.

4. **Görselleştirmeler**:
   - **Scatter Plot**: Satış miktarı ve birim fiyatı arasındaki ilişkiyi görselleştirdik.
   - **Histogram**: Toplam işlem değerinin dağılımını inceledik.
   - **Zaman Serisi Grafiği**: Zamanla birim fiyat ve satış miktarının değişimini gösterdik.
   - **Bar Graph**: Ürün kategorilerine göre ortalama toplam satış değerlerini görselleştirdik.

## Çıkarımlar ve Sonuçlar

- **Fiyat ve Satış Miktarı Arasındaki İlişki**: Fiyat ve satış miktarı arasında zayıf negatif bir ilişki gözlemlendi. Fiyat artışı, satış miktarını çok fazla etkilememektedir.
- **Satış Miktarı ve Toplam Satış Değeri**: Satış miktarı arttıkça toplam satış değeri de artmaktadır. Bu, satışların gelir üzerindeki olumlu etkisini göstermektedir.
- **Birim Fiyat ve Toplam Satış Değeri**: Fiyatın yükselmesiyle toplam satış değeri artmaktadır. Bu güçlü pozitif ilişki, yüksek fiyatların genellikle daha fazla gelir sağladığını göstermektedir.

## Görselleştirmeler

- **Scatter Plot**: Satış miktarı ve birim fiyatı arasındaki ilişkiyi görselleştirdik.
- **Histogram**: Toplam işlem değerinin dağılımını inceledik.
- **Zaman Serisi Grafiği**: Zamanla satış miktarı ve birim fiyatındaki değişimi gösterdik.
- **Bar Graph**: Ürün kategorilerine göre ortalama toplam satış değerlerini görselleştirdik.

