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


🔥 Новая архитектура BPS EXPRESS (Web3 + P2P + Блокчейн)
1️⃣ Web3-авторизация через OnchainKit
📌 Процесс авторизации:

    Пользователь нажимает «Войти через Web3».
    Вызов OnchainKit → появляется UI-окно с выбором кошелька (MetaMask, Coinbase Wallet, WalletConnect).
    Пользователь подключает кошелек → OnchainKit получает walletAddress.
    Генерируется уникальный onchain-токен (замена JWT).
    Данные пользователя записываются в локальное хранилище (или IPFS) для onchain-идентификации.
    WordPress получает информацию о сессии через API.
    Пользователь попадает в личный кабинет (Next.js + OnchainKit).
