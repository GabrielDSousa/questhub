# **QuestHub**

QuestHub is a modern web application designed to revolutionize learning through gamification and advanced memory retention techniques. With QuestHub, users can embark on personalized learning quests, complete engaging lessons, and track their progress with ease. Featuring a seamless integration of gamified learning mechanics, real-time progress tracking, and a dynamic user interface, QuestHub offers a unique and immersive learning experience for users of all skill levels. Join us on a journey of discovery and mastery with QuestHub.

---

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Authors](#authors)
- [License](#license)

---

## Code of Conduct

Please review our [Code of Conduct](CODE_OF_CONDUCT.md) before contributing to this project.

---

## Introduction

Our project aims to revolutionize learning by combining two powerful methodologies: gamification and the Anki method. Our web application provides users with a dynamic and engaging platform to master any subject or skill effectively. Through gamification, we transform the learning experience into an enjoyable journey, leveraging game-like elements to motivate and incentivize users to progress. Additionally, we integrate the scientifically proven Anki method, known for its effectiveness in memory retention, to optimize learning outcomes. By merging these methodologies, our goal is to empower users to learn efficiently and enjoyably, regardless of their proficiency level or area of interest.

---

## Prerequisites

To use QuestHub, you need to have the following software installed on your local development environment:

- [PHP 8.2+](https://www.php.net/)
- [Composer](https://getcomposer.org/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

---

## Installation

To use Sail in an existing Laravel application, you need to install it using the Composer package manager. Of course, these steps assume that your existing local development environment allows you to install Composer dependencies:

```bash
composer require laravel/sail --dev
```

Make a copy of the .env.example file and rename it to .env.

```bash
cp .env.example .env
```

After Sail has been installed, you can run the Artisan sail:install command. This command will publish the Sail docker-compose.yml file in the root of your application and modify your .env file with the necessary environment variables to connect to Docker services:

```bash
php artisan sail:install
```

For the desired functionality, choose the **mysql** and **mailpit** services.

Finally, you can start Sail.

```bash
./vendor/bin/sail up
```

Generate the application key.

```bash
./vendor/bin/sail artisan key:generate
```

Install project dependencies.

```bash
./vendor/bin/sail npm install
```

Compile the assets.

```bash
./vendor/bin/sail npm run build
```

Prepare the database.

```bash
./vendor/bin/sail artisan migrate
```

```bash
./vendor/bin/sail artisan db:seed key:generate
```

Test the system.

```bash
./vendor/bin/sail test
```

Access the application at [localhost](http://localhost).

To stop Sail, execute the following command.

```bash
./vendor/bin/sail down
```

The system is configured to send emails in a development environment. To view the sent emails, access Mailpit.

To access the Mailpit inbox, go to [localhost:8025](http://localhost:8025).

To generate an API access token, access the application frontend and log in. Then, go to the access token page.

Log in with the credentials of a created user or use the local development user:

- Email: <local@user.com>
- Password: password

---

## Usage [WIP]

Instructions on how to use the project, including examples and screenshots if applicable.

---

## Authors

- [Gabriel de Sousa](https://github.com/GabrielDSousa)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments [WIP]

Acknowledgments and credits to individuals or organizations that have contributed to the project.

---

**Note:** This README serves as a placeholder and will be updated with more detailed information as the project progresses.
