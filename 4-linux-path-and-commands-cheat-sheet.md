EN 🇬🇧
Command Types:

Internal (Built-in): Embedded inside the shell. Fast execution, no new process spawned (e.g., cd, source, fg).

External: Executable binaries located in directories like /bin or /usr/bin. Requires the shell to look up the PATH and spawn a new process (e.g., ls, cat, nano).

Checking Command Types & Locations:

type <command>: Identifies if a command is a shell builtin or external (e.g., type cd, type nano).

which <command>: Shows the exact binary path of an external command (e.g., which python3).

The PATH Variable:

echo $PATH: Displays a colon-separated list of directories where the system looks for external commands.

Add a custom directory to PATH: export PATH="/your/custom/dir:$PATH" (Allows running scripts/binaries globally without specifying their full path).

TR 🇹🇷
Komut Türleri:

Dahili (Internal/Built-in): Kabuğun (shell) kendi içine gömülüdür. Çok hızlı çalışırlar ve yeni bir süreç (process) başlatmazlar (Örn: cd, source, fg).

Harici (External): Genellikle /bin veya /usr/bin dizinlerinde bulunan çalıştırılabilir dosyalardır. Sistem PATH değişkenindeki yolları tarar ve yeni bir süreç başlatır (Örn: ls, cat, nano).

Komut Türü ve Konumu Sorgulama:

type <komut>: Komutun dahili mi yoksa harici mi olduğunu söyler (Örn: type cd, type nano).

which <komut>: Harici bir komutun tam olarak hangi dizinde (binary) olduğunu gösterir (Örn: which python3).

PATH Değişkeni:

echo $PATH: Harici komutların arandığı dizinlerin listesini (iki nokta : ile ayrılmış olarak) verir.

PATH'e Yeni Dizin Ekleme: export PATH="/yeni/dizin/yolu:$PATH" (Betik veya programları, tam dosya yolunu yazmadan her yerden doğrudan çalıştırmayı sağlar).
