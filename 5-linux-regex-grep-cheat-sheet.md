EN 🇬🇧
1. Regex Metacharacters
^ / $ : Matches the start / end of a line.

. : Matches any single character.

* / + / ? : Matches zero or more / one or more / zero or one of the preceding items.

[ ] / [^ ] : Matches any character inside / except the ones inside the brackets.

\ : Escape character used to treat special characters as literal text.

{n} / {n,m} : Matches exactly n / between n and m repetitions.

2. Essential grep Flags
-n : Displays line numbers with output.

-v : Inverts match (shows lines that do not match).

-i : Ignores case (case-insensitive).

-c : Prints only the count of matching lines.

-E : Enables Extended Regex (ERE), allowing modern syntax like |, +, ? without escaping.

3. Common Operations & Patterns
OR Logic: grep -E 'pattern1|pattern2' file (or standard grep: grep 'pattern1\|pattern2' file)

AND Logic: grep -E 'pattern1.*pattern2' file

Context Control (Before/After):

grep -A3 'pattern' file : Shows the match and 3 lines after it.

grep -B3 'pattern' file : Shows the match and 3 lines before it.

Chaining with xargs: ls | grep 'pattern' | xargs rm (Finds and deletes files matching a pattern).

TR 🇹🇷
1. Regex Özel Karakterleri
^ / $ : Satırın başlangıcını / bitişini ifade eder.

. : Herhangi bir tek karakterin yerini tutar.

* / + / ? : Kendinden önceki öğenin sıfır veya daha fazla / bir veya daha fazla / sıfır veya bir kez tekrarını yakalar.

[ ] / [^ ] : Köşeli parantez içindeki karakterlerden birini / parantez içindekiler hariç herhangi birini yakalar.

\ : Kaçış karakteridir; özel karakterleri düz metin olarak aratmak için kullanılır.

{n} / {n,m} : Kendinden önceki öğenin tam n kez / n ile m kez arasında tekrarını arar.

2. Temel grep Parametreleri
-n : Eşleşen satırların numarasını gösterir.

-v : Tersine eşleme yapar (eşleşmeyen satırları listeler).

-i : Büyük/küçük harf duyarlılığını kaldırır.

-c : Eşleşen toplam satır sayısını verir.

-E : Gelişmiş Regex (ERE) modunu açar; |, +, ? gibi karakterlerin ters eğik çizgi olmadan kullanılmasını sağlar.

3. Sık Kullanılan İşlemler ve Kalıplar
VEYA (OR) Mantığı: grep -E 'kalıp1|kalıp2' dosya (veya standart grep ile: grep 'kalıp1\|kalıp2' dosya)

VE (AND) Mantığı: grep -E 'kalıp1.*kalıp2' dosya

Bağlam Kontrolü (Öncesi/Sonrası):

grep -A3 'kalıp' dosya : Eşleşen satırı ve sonraki 3 satırı gösterir.

grep -B3 'kalıp' dosya : Eşleşen satırı ve önceki 3 satırı gösterir.

Xargs ile Komut Bağlama: ls | grep 'kalıp' | xargs rm (Kalıba uyan dosyaları bulur ve siler).
