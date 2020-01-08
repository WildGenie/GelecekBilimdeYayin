# Temiz ve Okunur Kodlama

[https://www.youtube.com/watch?v=HJJyV7rHvFk](https://www.youtube.com/watch?v=HJJyV7rHvFk)

Gelecek Bilimde tarafından sunulan, oyun içinde oyun serimizin 13. bölümü "Temiz ve Okunur Kodlama" yayınımızda işlemiş olduğumuz konu başlıkları

## Sözlük

**Code Smell:** Kod yapısındaki bazı düzensizlikler ve doğru yapılmamış implementasyonlar demektir. Temel olarak bunlar birer bug’dır diyemeyiz. Bunlar daha çok temel programlama prensiplerinin ihlalidir. Bir “code smell” temelde derinlerde yatan daha büyük bir sorunun göstergeleridir.

- **Technical Debt:** Bir şeyi hızlıca ve kolayca yapmanın ileride daha çok çalışma ve uğraş gerektirebileceğini kasteder. Bu konuda Martin Fowler - “Code Smell” ve Robert C. Martin’in “Clean Code” kitapları iyi bilinen dokumanlardır.
- **Code Refactoring:** Kodun kontrol ettiği davranışı değiştirmeden yapısını değiştirmektir. Programın fonksiyonel olmayan yerlerini temizlemeye, karmaşıklığı gidererek okunabilirliği arttırmaya, kaynak kodların bakım-onarıma elverişli (maintainability) hale getirmeye, kodun genişleyebilir hale getirmeye yarar.
- **Debugging**

## Kodlama Kuralları

### **Giriş Kuralları**

1- İnsan tarafından okunabilir olması.

2- İngilizce bilgisini arttırmak ve programdaki adların İngilizce yazılması.

3- Takım çalışması. Kodun nasıl yazılacağına karar vermek, editorconfig dosyası oluşturmak

### **Değişkenler Hakkında**

4- Değişken adları yeterince açıklayıcı ve telaffuz edilebilir olmalı. Değişken adında değişkenin türü prefix olarak yazılmamalı.

5- Aynı şeyden bahsederken aynı kelimeler kullanılmalı. Yani, aynı şeyi ifade etmek için bir yerde *user* diğerinde *player,* diğerinde *customer* denmemeli.

6- Değişken adında onun hangi kapsamda geçerli olduğu yazılmamalı.

7- Stringleri ve sayıları hardcoded olarak source code içinde yazmamalı.

### **Metot veya Fonksiyon Hakkında**

8- Bir metot ya da fonksiyon içinde, argümanlara ya da parametrelere değer verirken default değerleri kullanmayı ihmal etmemeli. Böylece fazladan bir karşılaştırma yapmaya gerek kalmaz.

9- Metot veya fonksiyonlarda, iki ya da daha az sayıda parametre ya da argüman kullanmak idealdir. Fakat bu programın yapısına göre değişiklik gösterebilir. Yine de bu kural akılda bulunmalıdır.

10- Fonksiyonlarda yan etki uygulamaktan kaçınmalı. Bir fonksiyon kendi alanı dışındaki bir değişkeni değiştirebiliyorsa, kod büyüdükçe ileride sorunlar çıkabilir. Bunun yerine o fonksiyona bir argüman vererek değiştirmek istediğimiz değeri ona göndermektir.

11- Bir fonksiyon bir iş yapmalı. Adı da yaptığı işi belirtmeli. Birden fazla iş yapan bir fonksiyon yerine sade bir şekilde bir işi yapan fonksiyon idealdir.

### **Yorum Kullanımı Hakkında**

12- Ne olduğu açık bir kod bloğu için yorum halinde açıklama yazılmamalı.

13- Yorum içerisinde programın tarihçesi tutulmamalı. Bunun yerine Git/Github vb. uygulamalarla versiyon kontrolü ve değişiklikler kontrol edilmeli.
14- Şeklinde pozisyon belirteci kullanılmamalı.