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
Konfigurasi default seluruh template, kecuali didefinisikan berbeda pada bagian `Daftar Template`.

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

### `centos7`

* default name: `centos7`
* box: `centos/7`
* hostname: `centos7.local`
* shared directory: `no shared directory!`

### `debian11`

* default name: `bullseye64`
* box: `debian/bullseye64`
* hostname: `bullseye.local`

### `fedora35`

* default name: `fedora35`
* box: `fedora/35-cloud-base`
* hostname: `fedora35.local`

### `rockylinux8`

* default name: `rockylinux8`
* box: `rockylinux/8`
* hostname: `rockylinux8.local`

### `ubuntu16`

* default name: `xenial`
* box: `bento/ubuntu-16.04`
* hostname: `xenial.local`
* memory: `2048`
* cpu: `2`

### `ubuntu22`

* default name: `jammy`
* box: `bento/ubuntu-22.04`
* hostname: `jammy.local`
* memory: `2048`
* cpu: `2`