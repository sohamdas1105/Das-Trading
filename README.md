
# Das Trading

## Overview
Das Trading is a Java Full Stack Crypto Trading platform that allows users to securely trade cryptocurrencies. The platform includes robust login authentication and integrates payment gateways such as Stripe and Razorpay for smooth and secure transactions with integrated AI chatbot.

## Features
- **User Authentication**: Secure login and registration using JWT tokens.
- **Crypto Trading**: Buy and sell cryptocurrencies in real-time.
- **Payment Integration**: Seamless transactions using Stripe and Razorpay.
- **Dashboard**: User-friendly interface to monitor your portfolio and trading activities.
- **Responsive Design**: Accessible on both desktop and mobile devices.

## Technologies Used
### Front-End
- HTML5
- CSS3
- JavaScript (ES6+)
- React.js

### Back-End
- Java
- Spring Boot
- Spring Security
- Hibernate (ORM)
- MySQL (Database)

### Payment Gateways
- Stripe
- Razorpay

### Other Tools and Libraries
- Maven
- JWT (JSON Web Tokens)
- Axios (for API requests)
- Docker (optional for containerized deployment)
  ### Comprehensive Feature Set


AI Chat Bot : Leverage our AI Chat Bot, designed to handle crypto-related queries like value of crypto and market data using Gemini API and CoinGecko API for real-time data.
Buy & Sell Crypto : Facilitate smooth crypto transactions with a user-friendly buy and sell interface, supporting a wide array of cryptocurrencies.
Portfolio Management: Equip your users with robust portfolio management tools to monitor investments and track performance

## Installation
### Prerequisites
- Java JDK 8 or higher
- Node.js and npm
- MySQL
- Docker (optional for containerized deployment)

### Back-End Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/das-trading.git
   cd das-trading/backend
   ```

2. Install dependencies:
   ```bash
   mvn install
   ```

3. Configure the database:
   - Create a MySQL database named `das_trading`.
   - Update the `application.properties` file in the `src/main/resources` directory with your database credentials:
     ```
     spring.datasource.url=jdbc:mysql://localhost:3306/das_trading
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     ```

4. Configure the environment variables:
   - Create an `application.properties` file in the `src/main/resources` directory.
   - Add the following environment variables:
     ```
     jwt.secret=your_jwt_secret
     stripe.api.key=your_stripe_api_key
     razorpay.api.key=your_razorpay_api_key
     razorpay.api.secret=your_razorpay_api_secret
     ```

5. Start the back-end server:
   ```bash
   mvn spring-boot:run
   ```

### Front-End Setup
1. Navigate to the `frontend` directory:
   ```bash
   cd ../frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Configure the environment variables:
   - Create a `.env` file in the `frontend` directory.
   - Add the following environment variables:
     ```
     REACT_APP_API_URL=http://localhost:8080/api
     REACT_APP_STRIPE_KEY=your_stripe_public_key
     REACT_APP_RAZORPAY_KEY=your_razorpay_public_key
     ```

4. Start the front-end development server:
   ```bash
   npm start
   ```

## Usage
1. Open your web browser and navigate to `http://localhost:3000`.
2. Register a new account or log in with an existing account.
3. Start trading cryptocurrencies and manage your portfolio through the dashboard.

## Docker Setup (Optional)
To run the application using Docker, follow these steps:

1. Ensure Docker is installed and running on your machine.

2. Clone the repository and navigate to the project directory:
   ```bash
   git clone https://github.com/yourusername/das-trading.git
   cd das-trading
   ```

3. Build and run the Docker containers:
   ```bash
   docker-compose up --build
   ```

4. Open your web browser and navigate to `http://localhost:3000`.

## Contributing
Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch-name`
3. Make your changes and commit them: `git commit -m 'Add new feature'`
4. Push to the branch: `git push origin feature-branch-name`
5. Create a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements
- Thanks to Stripe and Razorpay for providing the payment gateway APIs.
- Inspired by various online cryptocurrency trading platforms.

---

Feel free to modify the content as needed to better suit your project specifics.
