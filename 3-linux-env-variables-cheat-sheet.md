EN 🇬🇧
Local vs. Global Variables:

Local: Valid only within the current shell session. Not visible in env.

Global (Environment): Available to child processes and system-wide. Visible in env.

Variable Operations:

Create Local: MY_VAR="Value"

Create Global: export MY_VAR="Value" (or convert existing: export MY_VAR)

Print/Read: echo $MY_VAR

Delete/Remove: unset MY_VAR

Checking Variables:

env: Lists all global environment variables.

env | grep MY_VAR: Searches for a specific global variable.

TR 🇹🇷
Yerel (Local) vs. Global Değişkenler:

Yerel: Sadece mevcut terminal oturumunda geçerlidir. env komutunda görünmez.

Global (Ortam): Alt süreçler ve sistem genelinde erişilebilirdir. env çıktısında yer alır.

Değişken İşlemleri:

Yerel Tanımlama: MY_VAR="Değer"

Global Tanımlama: export MY_VAR="Değer" (veya yereli globale çevirme: export MY_VAR)

Ekrana Yazdırma: echo $MY_VAR

Silme/Kaldırma: unset MY_VAR

Değişkenleri Kontrol Etme:

env: Tüm global ortam değişkenlerini listeler.

env | grep MY_VAR: Belirli bir global değişkeni filtreleyip arar.
