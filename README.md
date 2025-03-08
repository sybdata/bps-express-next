# BPS EXPRESS — Web3 + P2P + Блокчейн =  Open Source 💙

<img width="508" alt="Image" src="https://bps.express/wp-content/uploads/2025/03/Screenshot-2025-03-02-212324.png" />

🚀 **BPS EXPRESS** — это инновационная платформа для заказа спортивной экипировки с использованием Web3-авторизации, хранения заказов в блокчейне и защиты отзывов от подделки.

## 🔥 Основные функции

### 1️⃣ Web3-авторизация

<img width="500" alt="Image" src="https://bps.express/wp-content/uploads/2025/02/Screenshot-2025-02-07-231406.png" />

**Процесс:**
- Пользователь нажимает «Войти через Web3».
- Вызов OnchainKit → UI-окно с выбором кошелька (MetaMask, Coinbase Wallet, WalletConnect).
- Пользователь подключает кошелек → OnchainKit получает `walletAddress`.
- Генерируется уникальный onchain-токен (замена JWT).
- Данные пользователя записываются в локальное хранилище (или IPFS) для onchain-идентификации.
- WordPress получает информацию о сессии через API.
- Пользователь попадает в личный кабинет (Next.js + OnchainKit).

### 2️⃣ Хранение заказов в блокчейне
**Процесс:**
- Клиент оформляет заказ.
- API связывает Next.js и Coinbase SDK.
- В блокчейн записываются ключевые данные:
  - Номер заказа
  - Дата покупки
  - Подтверждение реселлера
  - Статус доставки
- Клиент получает публичный хэш записи, подтверждающий неизменность данных.
- Полные детали хранятся в базе данных Supabase.

### 3️⃣ Подлинность отзывов в блокчейне
**Процесс:**
- Клиент оставляет отзыв → API проверяет, есть ли у него заказы.
- Отзыв записывается в блокчейн с уникальным ID.
- Отзывы невозможно удалить или изменить.
- Публичный хэш позволяет проверить подлинность отзыва.

### 4️⃣ Личный кабинет на Next.js
**Функционал:**
✅ История заказов (с блокчейн-хэшем)  
✅ Проверка статуса заказа  
✅ Доступ к отзывам и гарантиям  

## 🛠️ Технологический стек
- **Frontend:** Next.js + Tailwind CSS
- **Backend:** Node.js + Express/NestJS
- **База данных:** Supabase / PostgreSQL
- **Блокчейн:** Base (Ethereum L2)
- **Web3:** OnchainKit, Coinbase Wallet SDK
- **API:** REST API для взаимодействия с блокчейном и WordPress
- **Раздача контента:** Nginx (проксирование Next.js)

## 🏗 Архитектура проекта
✅ Web3-авторизация через OnchainKit (без паролей, через кошелек)  
✅ Фиксация заказов в блокчейне (гарантия подлинности)  
✅ Блокчейн-защита отзывов (нельзя подделать или удалить)  
✅ Прозрачный личный кабинет (Next.js + API)  
✅ WordPress управляет контентом (Next.js забирает данные через API)  

## 📌 Разработка и планы
- 🔄 **Текущий статус:** MVP в процессе реализации
- 🔜 **Планы:**
  - Поддержка NFT для VIP-доступа
  - Улучшенная система поиска товаров
  - AI-аналитика отзывов

📩 **Контакты для сотрудничества:** [bps-express.com](https://bps-express.com/)


# Next.js Web3 E-commerce Platform

A modern e-commerce platform built with Next.js, Supabase, and Web3 technologies.

## Features

- High-performance storefront with Next.js
- Web3 authentication using OnchainKit
- Cryptocurrency payments via Coinbase Commerce
- Verified reviews stored on Arweave
- Serverless backend with Supabase

## Technology Stack

- **Frontend:** Next.js, React, Tailwind CSS
- **Backend:** Supabase (PostgreSQL, API)
- **Authentication:** Web3 auth (OnchainKit)
- **Payments:** Coinbase Commerce
- **Hosting:** Vercel (frontend) + Supabase (database)
- **Reviews:** Arweave blockchain storage

## Getting Started

Instructions for setup and development coming soon.

## License

This project is licensed under the MIT License - see the LICENSE file for details.



