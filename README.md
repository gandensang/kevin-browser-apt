# Repositori APT Kevin Browser

Kevin Browser adalah peramban web ringan untuk Linux dengan RAM kecil:
tab tidur, pemblokir iklan dan pelacak, dan mesin pencari Google.
Repositori ini hanya berisi paket `.deb` dan indeksnya, yang disajikan
lewat GitHub Pages di <https://gandensang.github.io/kevin-browser-apt>.

Kode sumbernya terbuka (lisensi MIT), untuk siapa saja yang ingin
memeriksa apa yang dipasang di laptopnya atau ikut mengembangkan:
<https://github.com/gandensang/kevin-browser>.

## Memasang

Untuk Linux Mint 22 atau Ubuntu 24.04 ke atas, 64-bit. Jalankan di terminal:

    sudo wget -qO /usr/share/keyrings/kevin-browser.gpg https://gandensang.github.io/kevin-browser-apt/kevin-browser.gpg
    sudo wget -qO /etc/apt/sources.list.d/kevin-browser.sources https://gandensang.github.io/kevin-browser-apt/kevin-browser.sources
    sudo apt update
    sudo apt install kevin-browser

Setelah itu Kevin Browser ada di menu, dan bisa dibuka dari terminal:

    kevin-browser
    kevin-browser detik.com

Versi baru datang lewat Update Manager, bersama pembaruan lain.

Kalau sudah punya berkas `kevin-browser_…_amd64.deb`, cukup pasang berkas
itu dengan `sudo apt install ./kevin-browser_…_amd64.deb`. Alamat
repositori ini ikut terpasang, jadi versi berikutnya juga datang lewat
Update Manager.

## Melepas

    sudo apt purge kevin-browser

Alamat repositori dan kuncinya ikut terhapus. Riwayat dan data situs tetap
ada di `~/.local/share/kevin-browser`.
