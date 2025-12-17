# ArtGallery API 🎨

REST API для платформы, где художники могут выставлять свои картины с системой аутентификации и ролевым управлением.

## 🔧 Технологии
- **Backend**: Django + Django REST Framework
- **Аутентификация**: JWT + 2FA (TOTP через pyotp)
- **База данных**: PostgreSQL (по умолчанию Django ORM)
- **Дополнительно**: 
  - `pyotp` для двухфакторной аутентификации
  - `qrcode` для генерации QR-кодов
  - Система ролей и разрешений

## 🌟 Основные возможности
- 🔐 Безопасная аутентификация с JWT и 2FA
- 🖼 CRUD операции для художественных работ
- 👥 Ролевая система (художник, зритель, администратор)
- 📊 Логирование действий пользователей
- 🚪 Управление сессиями (мультисессионность)

## 🚀 Быстрый старт

### Предварительные требования
- Python 3.9+
- Django 4.0+
- Django REST Framework

### Установка
```bash
git clone https://github.com/Halstens/ArtGalleryAPI.git
cd art-gallery-api
pip install -r requirements.txt
python manage.py migrate
