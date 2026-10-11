<div align="center">

# Привет, я bylbozator

**Backend-разработчик (Python) и инженер по качеству.**

[![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-4169E1?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?logo=docker&logoColor=white)](https://docs.docker.com/compose/)
[![pytest](https://img.shields.io/badge/pytest-0A9EDC?logo=pytest&logoColor=white)](https://docs.pytest.org/)
[![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)](https://playwright.dev/)
[![GitHub Actions](https://img.shields.io/badge/CI-GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)](https://github.com/features/actions)

Пишу на **Python**, разворачиваю сервисы в **Docker**, автоматизирую процессы через **CI/CD**. Отношусь к качеству как к части разработки: пишу тесты, настраиваю мониторинг и держу проект документированным.

</div>

---

## Стек

```
Backend   ·  Python 3.11  ·  FastAPI  ·  SQLAlchemy 2.0  ·  Celery  ·  PostgreSQL  ·  Redis
Frontend  ·  React 18  ·  TypeScript  ·  Vite  ·  Tailwind CSS  ·  Univer.js
QA        ·  pytest  ·  Playwright E2E  ·  API-тестирование (Postman)  ·  тест-дизайн
DevOps    ·  Docker Compose  ·  Nginx  ·  Prometheus  ·  Grafana  ·  GitHub Actions  ·  Linux
```

## Ключевые проекты

### [pen-system-02](https://github.com/bylbozator/pen-system-02) — дипломный проект
Корпоративная система план/факт учёта и контроля поставок МТР. Полноценный full-stack продукт:

- **Backend:** Python 3.11, FastAPI, SQLAlchemy 2.0, Celery + Redis, PostgreSQL 15
- **Frontend:** React 18, TypeScript 5, Vite, Tailwind CSS 3, Univer.js (онлайн-редактор таблиц с формулами)
- **Фичи:** импорт/экспорт Excel и PDF, ролевая модель с JSON-разрешениями, аудит действий, JWT, rate limiting, WebSocket
- **Качество:** pytest (юнит + интеграционные), Playwright E2E, CI в GitHub Actions
- **Инфраструктура:** Docker Compose, Nginx, Prometheus + Grafana

[Первая версия проекта](https://github.com/bylbozator/pen-system) — прототип, на базе которого вырос pen-system-02.

### [moon-courier-crisis](https://github.com/bylbozator/moon-courier-crisis) — игровой симулятор
Браузерная игра (чистый JS + Canvas) с сервер-авторитативной симуляцией на Node:
**66 юнит-тестов** и **29 тестов REST API**, баланс откалиброван автопрогоном бота. Архитектура «чистый движок + слой хранения + UI» — движок переиспользуется браузером, сервером и тестами.

### [companies-data-case](https://github.com/bylbozator/companies-data-case) — работа с данными
Кейс обработки датасета ~1200 компаний «под ключ»:
- **ETL**: JSON → PostgreSQL (1000 записей, дедупликация, индексы `pg_trgm`, CHECK-констрейнты, 3 SQL-запроса);
- **Веб**: страница компаний на Next.js + TypeScript с поиском и фильтрами;
- **Качество данных**: аудит «грязного» CSV — 22 найденные аномалии, скрипт детекции;
- LLM-стек и принципы безопасности для coding-агентов.

### [wb-api-parser](https://github.com/bylbozator/wb-api-parser)
Приложение на Laravel: регулярная выгрузка продаж, заказов, остатков и доходов из API Wildberries-подобного сервиса в MySQL с обязательным SSL. Консольная команда `artisan app:fetch-api-data`, гибкая конфигурация через `.env`.

### [phishing-detector](https://github.com/bylbozator/phishing-detector) — информационная безопасность
Детектор фишинговых сайтов: проверка URL, разбор DOM через Selenium, оценка страницы локальной LLM и итоговый вердикт.

## DevOps

- [project-14-android-cicd](https://github.com/bylbozator/project-14-android-cicd) — сквозной CI/CD Android на GitHub Actions: build, lint, юнит-тесты с покрытием (JaCoCo), SonarQube-сканирование, публикация APK в JFrog Artifactory, уведомления в Teams, работа с AWS security groups.
- [project-03-linux-fundamentals](https://github.com/bylbozator/project-03-linux-fundamentals) — Linux Fundamentals для DevOps: пользователи и группы, права доступа, поиск, монтирование ФС. Все 11 фаз выполнены.
- [ib-lab-dvwa](https://github.com/bylbozator/ib-lab-dvwa) — лаборатория по уязвимому веб-приложению DWVA: разбор типовых уязвимостей веб-приложений.

## Низкоуровневое программирование

Лабораторные на ассемблере (TASM) — понимание того, как код отображается на регистры, память и прерывания:

- [asm-bresenham-cylinder](https://github.com/bylbozator/asm-bresenham-cylinder) — графика в VESA 800×600: алгоритмы Брезенхема для линии и окружности;
- [asm-overlay-arithmetic-calculator](https://github.com/bylbozator/asm-overlay-arithmetic-calculator) — калькулятор арифметических выражений с оверлейными функциями;
- [asm-reverse-string](https://github.com/bylbozator/asm-reverse-string) / [asm-reverse-string-cpp](https://github.com/bylbozator/asm-reverse-string-cpp) — реверс строки на TASM и на C++.

## В процессе

- Осваиваю публичную программу [DevOps-Projects](https://github.com/DevCloudNinjas/DevOps-Projects): 52 практических проекта от Linux и Terraform до EKS, Argo CD и DevSecOps (Kubernetes, Terraform, Argo CD, DevSecOps — по мере готовности выкладываю репозитории).