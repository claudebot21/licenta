# SmartHome

SmartHome este o aplicatie ce are rolul de a oferi un singur dashboard pentru device-uri bazate pe servicii diferite. De asemenea, a fost proiectul meu de licenta.

## Demo - dezactivat temporar
Demo: https://licenta.dekolor.ro/

User: test@dekolor.ro

Pass: test123

*In demo nu se poate porni/opri pe bune un device si nici automatizarile nu modifica starea acestuia.*

## Requirements

- PHP 7.3+ sau PHP 8.0+
- MySQL/MariaDB
- Composer
- Web server (Apache/Nginx)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/dekolor/licenta.git
cd licenta
```

2. Install dependencies:
```bash
composer install
```

3. Configure environment:
```bash
cp env .env
# Edit .env with your database credentials
```

4. Import database schema:
```bash
mysql -u username -p database_name < db.sql
```

5. Point your webserver to the `/public` folder

6. Set up cron job for automation:
```bash
* * * * * curl https://your-domain.com/cron/run >/dev/null 2>&1
```

## Configuration

Copy `env` to `.env` and configure:
- Database credentials
- App base URL
- Environment (development/production)

**⚠️ Important:** Never commit `.env` to git! It contains sensitive data.

## Features

- 📱 Dashboard pentru control device-uri IoT
- 🏠 Suport multi-platformă (dispozitive de la vendori diferiți)
- ⏰ Automatizări bazate pe timp sau apus/răsărit
- 👥 Management utilizatori
- 📝 Logging acțiuni
- 🔐 Autentificare securizată

## Screenshots

### Dashboard
![](https://i.imgur.com/RGBxvsg.png)

### Lista device-uri
![](https://i.imgur.com/R6AQebt.png)

### Lista automatizari
![](https://i.imgur.com/2nc3Mny.png)

### Adaugarea unei automatizari
![](https://i.imgur.com/Cv7h2hm.png)

### Lista de utilizatori
![](https://i.imgur.com/99LZTNk.png)

### Setari
![](https://i.imgur.com/8oi8AzPK.png)

## Security

Daca descoperiti vulnerabilitati, va rog sa le raportati prin email la stefan@dekolor.ro

## License

MIT License
