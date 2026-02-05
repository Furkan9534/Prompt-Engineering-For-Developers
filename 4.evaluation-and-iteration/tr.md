# Prompt Evaluation and Iteration

Bu bölümde prompt tasarımının
nasıl sistematik olarak değerlendirileceği
ve nasıl geliştirileceği anlatılmaktadır.

Amaç:
prompt geliştirme sürecini deneme–yanılma seviyesinden
mühendislik sürecine taşımaktır.

---

## Neden değerlendirme gerekir?

Bir promptun “iyi” olması,
tek bir örnekte doğru cevap üretmesi anlamına gelmez.

Gerçek sistemlerde aşağıdaki problemler ortaya çıkar:

- aynı prompt farklı çalıştırmalarda farklı kalitede sonuç üretir
- çıktı formatı bozulur
- model zaman zaman uydurma bilgiler üretir

Bu nedenle promptlar ölçülmeden geliştirilemez.

---

## Temel değerlendirme metrikleri

Her prompt için en az aşağıdaki metrikler izlenmelidir.

| Metrik | Açıklama |
|------|-------|
| Correctness | Sonuçlar görev açısından doğru mu? |
| Consistency | Benzer girdilerde benzer çıktı üretiyor mu? |
| Format stability | Çıktı şablonu korunuyor mu? |
| Hallucination risk | Uydurma bilgi veya kaynak var mı? |
| Coverage | Tüm alt gereksinimleri kapsıyor mu? |

---

## Basit değerlendirme protokolü

Önerilen minimum süreç:

1. temsil edici test girdileri oluştur
2. her girdi için çıktıları kaydet
3. metriklere göre işaretle
4. zayıf noktaları analiz et
5. promptu yeniden tasarla

---

## Prompt versiyonlama

Gerçek projelerde promptlar:

- kod gibi
- versiyonlanmalıdır.

Önerilen yaklaşım:

- her büyük değişiklik için prompt v1, v2, v3 etiketleri
- değişiklik notlarının tutulması
- hangi versiyonun nerede kullanıldığının belirtilmesi

---

## Prompt loglama

API ile çalışan sistemlerde:

- kullanılan prompt
- model ayarları
- zaman
- girdi / çıktı

kayıt altına alınmalıdır.

Bu kayıtlar:

- hata analizi
- kalite takibi
- regresyon testleri

için gereklidir.

---

## İteratif geliştirme döngüsü

Bu repo boyunca önerilen döngü:

Design → Run → Evaluate → Refine

Bu döngü,
model veya prompt değiştikçe
sürekli olarak uygulanmalıdır.
