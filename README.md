# Koleksi template `vagrant` 

## Tentang
Koleksi template vagrant untuk keperluan belajar dan pengembangan.

## Penggunaan
Salin template ke direktori `deployment` lalu jalankan `vagrant up`.

NOTE: **UBAH KONFIGURASI `vb.name` SEBELUM MENJALANKAN**
```bash
# Contoh untuk menjalankan jika menggunakan shell `bash`
cp -r alpine312 deployment/alpine312-project0
cd deployment/alpine312-project0
# ubah konfigurasi `vb.name``
vagrant up

# Contoh untuk mematikan
cd deployment/alpine312-project0
vagrant halt
```

## Default Konfigurasi
Konfigurasi default seluruh template, kecuali didefinisikan lain pada bagian `Daftar Template`.

* provider: `virtualbox`
* network: `bridge`
* shared directory:
    * host: `./shared_data` 
    * guest: `/vagrant_data`
* memory: `1024`
* cpu: `1`

## Daftar Template

### `alpine312`

* default name: `alpine312`
* box: `generic/alpine312`
* hostname: `alpine312.local`

### `debian11`

* default name: `bullseye64`
* box: `debian/bullseye64`
* hostname: `bullseye.local`