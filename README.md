# Laravel Reverb Real-Time Chat App

A real-time chat application built using Laravel and Laravel Reverb. This project uses Laravel UI with React for the frontend and provides real-time message broadcasting using Laravel Reverb.

## 🚀 Features

- Real-time messaging
- Laravel Reverb integration
- Authentication scaffolding with React
- Queue workers and event broadcasting

---

## 🛠 Installation

Follow the steps below to set up the Laravel Reverb-powered chat app:

### 1. Create a New Laravel Project

```bash
composer create-project laravel/laravel-chat-app
cd laravel-chat-app

php artisan make:model -m Message
php artisan migrate:fresh
composer require laravel/ui
php artisan ui react --auth
npm install 
npm run build
php artisan optimize
php artisan serve
npm run dev
php artisan make:event GotMessage
php artisan make:job SendMessage
php artisan install:broadcasting
php artisan queue:listen
php artisan reverb:start


OR 

click the below links and read the documents carefully

https://www.freecodecamp.org/news/laravel-reverb-realtime-chat-app/