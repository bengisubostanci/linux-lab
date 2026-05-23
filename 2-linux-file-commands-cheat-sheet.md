EN 🇬🇧
Directory & File Operations:

mkdir -p path/to/dir: Creates nested directories recursively.

pwd: Prints current working directory.

touch filename: Creates an empty file or updates timestamps.

Listing Files (ls Flags):

ls -l: Detailed long list.

ls -lh: Human-readable file sizes (e.g., 12K).

ls -lS: Sorts by file size.

ls -lt: Sorts by modification time (newest first).

ls -lr: Reverses sorting order (e.g., -ltr sorts by time, oldest first).

ls -la: Shows all files, including hidden ones (starting with a .).

Navigation (cd):

cd .. / cd ../..: Move up 1 or 2 directory levels.

cd ~ / cd /: Go to Home directory / Root directory.

Command History:

history 5: Lists the last 5 executed commands.

history -c: Clears the command history.

Aliases:

Temporary: alias myll="ls -ltr" (Lasts until session ends).

Permanent: Add alias myll="ls -ltr" into ~/.bashrc, then reload using source ~/.bashrc.

TR 🇹🇷
Dizin & Dosya İşlemleri:

mkdir -p yol/dizin: İç içe geçmiş dizinleri tek seferde oluşturur.

pwd: Mevcut çalışma dizinini gösterir.

touch dosya_adi: Boş bir dosya oluşturur veya zaman damgasını günceller.

Dosya Listeleme (ls Parametreleri):

ls -l: Detaylı uzun liste.

ls -lh: Dosya boyutlarını okunabilir formatta gösterir (Örn: 12K).

ls -lS: Dosya boyutuna göre büyükten küçüğe sıralar.

ls -lt: Değişiklik zamanına göre sıralar (en yeni en başta).

ls -lr: Sıralamayı tersine çevirir (Örn: -ltr zamana göre en eski en başta).

ls -la: Gizli dosyalar (. ile başlayanlar) dahil tümünü listeler.

Dizin Değiştirme (cd):

cd .. / cd ../..: 1 veya 2 üst dizine çıkar.

cd ~ / cd /: Home (Ev) dizinine / Root (Kök) dizinine gider.

Komut Geçmişi (history):

history 5: Son çalıştırılan 5 komutu listeler.

history -c: Tüm komut geçmişini temizler.

Takma Adlar (Alias):

Geçici: alias myll="ls -ltr" (Oturum kapanana kadar geçerli).

Kalıcı: ~/.bashrc dosyasının içine alias myll="ls -ltr" satırını ekle ve source ~/.bashrc komutu ile aktif et.
