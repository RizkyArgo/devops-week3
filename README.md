# Latihan Docker – DevOps Week 3

Repository ini berisi latihan dasar Docker dalam program belajar DevOps mingguan. Fokus latihan adalah memahami Dockerfile, container, serta konsep layering image.

## Struktur Direktori

```
.
├── day5-copy/
│   ├── Dockerfile
│   ├── a.txt
│   ├── b.txt
│   └── c.txt
├── day6-layering/
│   ├── Dockerfile
│   ├── a.txt
│   ├── b.txt
├── day7-folder-copy/
│   ├── Dockerfile
│   └── src/
│       └── pesan.txt
```

## Rangkuman Latihan

### Day 5 – Copy Beberapa File
- Menyalin beberapa file (`a.txt`, `b.txt`, `c.txt`) ke dalam container menggunakan Dockerfile.
- Memahami perintah `COPY` dan struktur direktori build.

### Day 6 – Layering dan Build Ulang
- Mengubah isi file dan membangun ulang image dengan `--no-cache`.
- Memahami bagaimana Docker membagi proses build menjadi beberapa layer.
- Belajar pentingnya urutan instruksi dalam Dockerfile.

### Day 7 – Struktur Folder dan Copy dari Subfolder
- Menyalin file dari subfolder `src/` ke dalam container.
- Mengatur `WORKDIR` dan `CMD` agar path file dapat diakses dengan benar.

## Perintah Penting

```bash
docker build -t nama-image .
docker run --rm nama-image
docker ps -a
docker start container_id
docker exec -it container_id sh
docker stop container_id
```

Catatan: Semua latihan menggunakan Docker berbasis Alpine dan Ubuntu untuk simulasi ringan dan cepat.

Dibuat oleh Rizky Argo
