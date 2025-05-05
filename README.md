# User Management - Laravel + React

Sistem manajemen pengguna menggunakan **Laravel** untuk backend dan **React (Vite)** untuk frontend.

## 🚀 Dokumentasi Instalasi

### 1. Prasyarat

Pastikan Anda telah menginstal:

- PHP ≥ 8.1
- Composer
- Node.js ≥ 18 dan npm
- MySQL (atau database lain yang kompatibel)
- Git

---

### 2. Clone Repository

```bash
git clone https://github.com/Chrisdiantodoni/user-management.git
cd user-management
```

### 3. Instalasi Backend (Laravel)
bash
Copy
Edit
cd backend/user-management-api
composer install
cp .env.example .env
php artisan key:generate
Lalu konfigurasikan database Anda di file .env:

env
Copy
Edit
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database
DB_USERNAME=root
DB_PASSWORD=your_password
Migrasi dan seed database:

bash
Copy
Edit
php artisan migrate
php artisan db:seed
Jalankan server Laravel:

bash
Copy
Edit
php artisan serve
4. Instalasi Frontend (React)
bash
Copy
Edit
cd ../../front-end/user-management-react
npm install --legacy-peer-deps
Jalankan development server:

bash
Copy
Edit
npm run dev
5. Jalankan Project
Laravel Backend berjalan di: http://127.0.0.1:8000

React Frontend (Vite) biasanya di: http://localhost:5173

⚠️ Pastikan CORS dan proxy sudah diatur jika frontend melakukan request ke API backend.

6. Troubleshooting Umum
Jika muncul error seperti vite is not recognized, pastikan Vite sudah diinstal secara global atau gunakan:

bash
Copy
Edit
npx vite
Pastikan file .env pada backend sudah dikonfigurasi dengan benar.

📂 Struktur Direktori
sql
Copy
Edit
user-management/
├── backend/
│   └── user-management-api/   # Laravel project
└── front-end/
    └── user-management-react/ # React project
📄 Lisensi
Project ini menggunakan lisensi MIT.

go
Copy
Edit

README ini sudah siap langsung ditempatkan di root repo `user-management`. Ingin saya bantu generate `proxy` config juga untuk React-nya?
