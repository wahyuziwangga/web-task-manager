# Web Task Manager

Aplikasi manajemen tugas berbasis web menggunakan Flask dan PostgreSQL yang dijalankan dengan Docker Compose.

## Teknologi

- **Flask** - Python web framework
- **PostgreSQL** - Database
- **Docker Compose** - Container orchestration

## Struktur Project

```
web-task-manager/
├── app/
│   ├── Dockerfile
│   ├── main.py
│   ├── requirements.txt
│   └── templates/
│       ├── index.html
│       └── task.html
├── db/
│   └── init.sql
├── docker-compose.yaml
└── README.md
```

## Cara Menjalankan

### Pertama kali / ada perubahan kode

```bash
docker compose up -d --build
```

### Sehari-hari

```bash
docker compose up -d    # jalankan
docker compose stop     # hentikan
```

### Cek status container

```bash
docker compose ps
docker compose logs -f
```

## Akses Aplikasi

| Service | URL |
|---------|-----|
| Web App | http://localhost:5000 |
| PostgreSQL | localhost:5432 |

## Fitur

- Tambah tugas
- Edit tugas
- Hapus tugas
- Lihat semua tugas
