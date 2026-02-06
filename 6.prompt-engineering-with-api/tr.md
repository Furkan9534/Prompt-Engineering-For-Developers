# API ile Prompt Engineering

Bu bölüm, promptların uygulama içinde
nasıl yönetilmesi gerektiğini açıklar.

Amaç:
promptları sabit string olarak değil,
konfigürasyon ve sistem bileşeni olarak ele almaktır.

---

## Prompt template kavramı

Gerçek sistemlerde promptlar:

- değişken alanlar (slots) içeren
şablonlar olarak tasarlanmalıdır.

Örnek kavramlar:

- {user_question}
- {schema}
- {context}

---

## Prompt yönetimi

Önerilen pratikler:

- promptları ayrı dosyalarda tutmak
- uygulama kodu ile karıştırmamak
- prompt versiyonlarını takip etmek

---

## Model parametrelerinin önemi

Aynı prompt:

- temperature
- top_p
- max_tokens

gibi ayarlara göre farklı davranabilir.

Bu nedenle prompt değerlendirmesi yapılırken
model konfigürasyonu da sabitlenmelidir.

---

## Ortam bazlı kullanım

Geliştirme ve üretim ortamlarında:

- farklı prompt versiyonları
- farklı model ayarları

kullanılması gerekebilir.

Bu ayrım açık şekilde yönetilmelidir.
