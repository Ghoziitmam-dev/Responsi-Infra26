# Analisis Perbaikan

## Permasalahan 1

### Gejala
Eror pada docker-compose.yml

### Penyebab
ada typo pada service
Nama volume tidak konsisten
Host database salah
typo pada folder web3
Network belum didefinisikan
### Solusi
Perbaiki menjadi:
services:

volumes:
  db-data:

ubah menjadi 
context: ./web3

Tambahkan:

networks:
  frontend:
  backend:


## Permasalahan 2

### Gejala
Error pada web1

### Penyebab
Typo pada dockerfile

### Solusi
perbaiki menjadi tulisan apache

## Permasalahan 3

### Gejala
Error pada web3

### Penyebab
Typo pada dockerfile

### Solusi
perbaiki menjadi tulisan apache

## Permasalahan 4

### Gejala
Error pada db

### Penyebab
ada markdown pada folder init.sql

### Solusi
hapus markdown dan hilangkan tulisan sql

## Permasalahan 4

### Gejala
Error pada nginx

### Penyebab
ada markdown di file nginx.conf
web1 ditulis web11
ada tulisan nginx
### Solusi
hapus markdown
perbaiki menjadi web1
hapus tulisan nginx
