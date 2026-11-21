# Smarter Patrols

**Yazar**: Monsterfish
**Sürüm**: 1.0.1

Yapay zekânın devriye ve kuşatma koruma birliklerinin bir saldırı sırasında tüm gruplarını gerçekten kullanmasını sağlar. Her iki bölüm de ayarlardan ayrı ayrı kapatılabilir.

## Devriye birlikleri

Normal oyunda yalnızca ilk devriye grubu emir alır. İkincisi tüm saldırı boyunca toplanma noktasında bekler.

Bu modülle her devriye grubu saldırılan kalenin çevresinde kendi rotasına sahip olur:

- **1. grup** kalenin etrafında bir yönde döner.
- **2. grup** ters yönde döner.
- **3. grup** kalenin ön cephesi (saldırana bakan taraf) boyunca gidip gelir.
- **4., 5. ve 6. gruplar** 1., 2. ve 3. ile aynı rotayı çeyrek tur geriden izler; 7., 8. ve 9. gruplar da onların arkasından gelir.

Kalenin dışında belirli bir yürüme mesafesinde dolaşırlar (varsayılan 12 kare; oyunun kendi devriyesiyle aynı), böylece surlara ve hendeklere dalmak yerine etraflarından dolanırlar. Düşmanla karşılaşan grup önce savaşır, sonra yoluna devam eder.

## Kuşatma koruma birlikleri

Bu birlikler zaten bir kuşatma aracından diğerine yürür, ancak her iki grup da aynı anda aynı rotayı izlediği için tek bir grup gibi görünürler.

Bu modülle:

- Her grup farklı bir kuşatma aracında başlar ve her ikinci grup ters yönde yürür; böylece tüm araçlara yayılırlar.
- Ağırlıklı olarak yakın dövüş birliklerinden oluşan gruplar, savunmacıların ateşini kuşatma araçları yerine üzerlerine çekmek için araçların birkaç kare önünde (kaleye doğru) yürür. Okçular araçların yanında kalır.
- Surlara saldırı başladığında her grup, normal oyunda olduğu gibi hücuma katılır.

## Daha fazla grup

Oyun tek başına yalnızca 2 devriye grubu ve 2 kuşatma koruma grubu yönetebilir. Bir yapay zekâ dosyası daha fazlasını isterse fazla birimler yanlış birliklere (hendek kazıcılara veya ana orduya) gider. Bu modül her birinden 12 gruba kadar destekler. Sayı, ayarlardan özel bir değer verilmedikçe yapay zekânın kendi dosyasından alınır (kuşatma koruması varsayılan: 4). Bir birlik yalnızca her grupta en az 4 birim kalacak şekilde bölünür (değiştirilebilir).

Ek gruplar yalnızca ordu saldırıdayken var olur. Surda gedik açıldığında, lord öldüğünde veya yapay zekâ geri çekildiğinde tekrar diğerleriyle birleşip yapay zekânın normal emirlerini izlerler.

## Bilmeniz gerekenler

- Yalnızca yapay zekâ saldırıları etkilenir; kendi birliklerinize dokunulmaz.
- Lord Hunt ile uyumludur.
- Kayıt dosyalarına fazladan hiçbir veri yazılmaz.
