# Foundations – Prompt Tasarımının Temelleri

Bu bölümde, tüm repo boyunca kullanılacak olan
temel prompt tasarım yaklaşımı tanıtılır.

Amaç, tek seferlik iyi cevap almak değil;
kontrol edilebilir ve tekrar üretilebilir çıktılar elde etmektir.

---

## Neden bir temel yapıya ihtiyacımız var?

Gerçek sistemlerde prompt’lar genellikle:

- belirsizdir
- farklı kişiler tarafından yazılır
- zaman içinde değiştirilir
- API üzerinden çalıştırılır

Bu durumda aşağıdaki problemler ortaya çıkar:

- modelin rolü net değildir
- görevin sınırları belirsizdir
- hangi bilginin kullanılacağı açık değildir
- çıktı formatı kararsızdır

Bu nedenle prompt tasarımı,
serbest metin yazımı gibi ele alınamaz.

---

## Temel tasarım ilkeleri

Bu repo boyunca şu ilkeler kullanılacaktır:

### 1. Açıklık (Clarity)

Modelden ne istendiği,
tek bir cümleyle bile yanlış anlaşılmayacak şekilde belirtilmelidir.

---

### 2. Sınırların belirlenmesi (Boundaries)

Modelin:

- hangi konunun içinde kalacağı
- hangi varsayımları yapabileceği
- hangi bilgileri kullanabileceği

net olarak tanımlanmalıdır.

---

### 3. Yapısallık (Structure)

Prompt,
paragraflardan oluşan bir metin değil,
bölümlere ayrılmış bir tasarım dokümanı gibi ele alınmalıdır.

---

### 4. Çıktı kontrolü (Output control)

Üretilen çıktı:

- otomatik sistemlere verilebilir olmalı
- formatı kararlı olmalı
- mümkünse makine tarafından ayrıştırılabilir olmalıdır

---

## Prompt tasarımı bir arayüzdür

Bir prompt,
model ile uygulama arasındaki arayüzdür.

Yanlış tasarlanmış bir arayüz:

- hatalı kullanım üretir
- kararsız davranışa yol açar
- sistemin bakım maliyetini artırır

Bu nedenle prompt,
API sözleşmesi (contract) gibi düşünülmelidir.

---

## En küçük anlamlı yapı

Bu repoda en küçük anlamlı prompt yapısı şu dört bileşenden oluşur:

- Role
- Task
- Context
- Output

Bu yapı:

sonraki bölümlerde kullanılacak olan
tüm prompt pattern’lerinin temelini oluşturur.

Bu bileşenlerin ayrıntılı açıklaması
`role-task-context-output` klasöründe yapılacaktır.

---

## Prompt tasarımı bir iterasyon sürecidir

İyi bir prompt:

ilk denemede bulunmaz.

Aşağıdaki döngü sürekli olarak uygulanmalıdır:

1. tasarla
2. çalıştır
3. değerlendir
4. iyileştir

Bu döngü,
ilerideki “evaluation and iteration” bölümünde
daha sistematik olarak ele alınacaktır.

---

## Bu bölümden sonra ne öğreneceksin?

Bu bölümden sonra:

- bir promptu parçalara ayırarak tasarlayabilecek
- rol, görev, bağlam ve çıktı kavramlarını net biçimde ayırabilecek
- promptları sürdürülmesi mümkün yapılar haline getirebileceksin
