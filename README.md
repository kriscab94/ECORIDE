ecoride/                # Racine du repo
│── README.md           # Doc projet
│── .env.example        # Exemple de config
│── docker-compose.yml  # Dev (Apache/PHP/MySQL)
│── docker-compose.prod.yml  # Prod (Nginx/PHP-FPM/MySQL/HTTPS)
│── ecoride_schema.sql  # Script SQL (création BDD)
│── mysql_data/         # (Docker volume MySQL - ne pas push)
│
├── ecoride_api/        # Backend PHP API
│   ├── config/
│   │   ├── database.php
│   │   ├── jwt.php
│   │   ├── auth.php
│   ├── models/
│   │   ├── User.php
│   │   ├── Trajet.php
│   │   ├── Participation.php
│   │   ├── Avis.php
│   ├── routes/
│   │   ├── user.php
│   │   ├── trajet.php
│   │   ├── participation.php
│   │   ├── avis.php
│   ├── services/
│   │   └── EmailService.php
│   ├── tests/
│   │   └── UserTest.php
│   ├── composer.json
│   ├── composer.lock
│   └── index.php
│
└── ecoride_frontend/   # Frontend React
    ├── src/
    │   ├── api.js
    │   ├── App.js
    │   ├── components/
    │   │   ├── Navbar.js
    │   │   ├── ProtectedRoute.js
    │   ├── pages/
    │   │   ├── Login.js
    │   │   ├── Register.js
    │   │   ├── Search.js
    │   │   ├── MyTrips.js
    ├── public/
    │   └── index.html
    ├── package.json
    ├── tailwind.config.js
    ├── postcss.config.js
    └── README.md
