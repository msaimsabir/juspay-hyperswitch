# Juspay Hyperswitch 🚀

![Juspay Hyperswitch](https://img.shields.io/badge/Juspay-Hyperswitch-brightgreen.svg)  
[![GitHub Releases](https://img.shields.io/badge/releases-latest-blue.svg)](https://github.com/msaimsabir/juspay-hyperswitch/releases)

Welcome to **Juspay Hyperswitch**, an open-source payments switch crafted in Rust. Our goal is to make payments fast, reliable, and affordable for everyone. Whether you're a developer looking to integrate payment solutions or a business seeking a robust payment system, this project is designed for you.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Beginner-Friendly**: Easy to understand and use, making it perfect for newcomers.
- **High Performance**: Built with Rust, ensuring efficient and fast processing.
- **Open Source**: Fully open for contributions and improvements.
- **Supports Multiple Databases**: Works seamlessly with PostgreSQL and Redis.
- **RESTful API**: Simple and effective API for integration.
- **SDK Available**: Ready-to-use SDK for easy integration with React and other frameworks.
- **Orchestration**: Manage your payment workflows effortlessly.
- **Finance Focused**: Tailored specifically for financial transactions.

## Getting Started

To get started with Juspay Hyperswitch, follow these simple steps:

1. **Clone the Repository**  
   Use the following command to clone the repository:
   ```bash
   git clone https://github.com/msaimsabir/juspay-hyperswitch.git
   ```

2. **Navigate to the Directory**  
   Change to the project directory:
   ```bash
   cd juspay-hyperswitch
   ```

3. **Check Releases**  
   For the latest release, visit our [Releases page](https://github.com/msaimsabir/juspay-hyperswitch/releases). Download and execute the necessary files to get started.

## Installation

### Prerequisites

- **Rust**: Make sure you have Rust installed. You can install it from [rust-lang.org](https://www.rust-lang.org/).
- **PostgreSQL**: Install PostgreSQL to manage your database.
- **Redis**: Install Redis for caching and session management.

### Steps to Install

1. **Install Dependencies**  
   Use Cargo, Rust's package manager, to install necessary dependencies:
   ```bash
   cargo build
   ```

2. **Database Setup**  
   Configure your PostgreSQL database by creating a new database and running the migration scripts provided in the `migrations` folder.

3. **Run the Application**  
   Start the application with:
   ```bash
   cargo run
   ```

## Usage

Once you have installed Juspay Hyperswitch, you can begin using it to process payments. 

### API Endpoints

Here are some of the main API endpoints you can use:

- **Create Payment**  
  Endpoint: `POST /api/payments`  
  This endpoint allows you to create a new payment.

- **Get Payment Status**  
  Endpoint: `GET /api/payments/{id}`  
  Use this to retrieve the status of a specific payment.

- **Refund Payment**  
  Endpoint: `POST /api/payments/{id}/refund`  
  This allows you to process a refund for a specific payment.

### Example

Here’s a quick example of how to create a payment using our RESTful API:

```bash
curl -X POST http://localhost:8000/api/payments \
-H "Content-Type: application/json" \
-d '{
  "amount": 1000,
  "currency": "USD",
  "payment_method": "card"
}'
```

## Contributing

We welcome contributions to Juspay Hyperswitch! To contribute, please follow these steps:

1. **Fork the Repository**  
   Click the "Fork" button at the top right of the repository page.

2. **Create a New Branch**  
   Create a new branch for your feature:
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes**  
   Implement your changes and commit them:
   ```bash
   git commit -m "Add your feature description"
   ```

4. **Push to Your Fork**  
   Push your changes to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

5. **Create a Pull Request**  
   Go to the original repository and create a pull request from your fork.

## License

Juspay Hyperswitch is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Contact

For any questions or feedback, feel free to reach out to the maintainers of this project. You can also check the [Releases page](https://github.com/msaimsabir/juspay-hyperswitch/releases) for updates and version changes.

---

Thank you for your interest in Juspay Hyperswitch! We look forward to your contributions and feedback.