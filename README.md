<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Digital Currency Platform - SRS</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f7fc;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #1E2A8A;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        section {
            padding: 20px;
            margin: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            animation: fadeIn 1s ease-in-out;
        }
        h1, h2 {
            color: #1E2A8A;
        }
        h3 {
            color: #5e5e5e;
        }
        ul {
            padding-left: 20px;
        }
        li {
            margin: 8px 0;
        }
        footer {
            text-align: center;
            background-color: #1E2A8A;
            color: white;
            padding: 10px 0;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        /* Simple animation */
        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }
        .highlight {
            color: #e91e63;
        }
    </style>
</head>
<body>
    <header>
        <h1>Digital Currency Platform - Software Requirement Specification (SRS)</h1>
    </header>

    <section>
        <h2>1. Introduction</h2>
        <h3>1.1 Purpose</h3>
        <p>This document outlines the requirements and specifications for building a <span class="highlight">Digital Currency Platform</span>. The platform will allow users to buy, sell, and transfer a custom digital currency (similar to cryptocurrency) and will integrate with real payment gateways like Razorpay. The platform will also include face scan authentication for withdrawals, ensuring security.</p>

        <h3>1.2 Scope</h3>
        <p>The Digital Currency Platform will support the following key features:</p>
        <ul>
            <li><strong>Coin Purchase:</strong> Users can purchase the digital currency using real money (via Razorpay).</li>
            <li><strong>Wallet System:</strong> Users will have a digital wallet to store their coins.</li>
            <li><strong>Transaction System:</strong> Users can send and receive coins from other users.</li>
            <li><strong>Blockchain Simulation:</strong> All transactions will be recorded in a blockchain-like structure for transparency.</li>
            <li><strong>Face Scan Authentication:</strong> Used for secure login and withdrawal authorization.</li>
            <li><strong>Admin Dashboard:</strong> Admins will manage user transactions and monitor activities.</li>
        </ul>

        <h3>1.3 Definitions, Acronyms, and Abbreviations</h3>
        <ul>
            <li><strong>API:</strong> Application Programming Interface</li>
            <li><strong>JWT:</strong> JSON Web Token (used for authentication)</li>
            <li><strong>MongoDB:</strong> NoSQL database used for storing data</li>
            <li><strong>Razorpay:</strong> Payment gateway for transactions</li>
            <li><strong>Blockchain:</strong> A decentralized ledger for recording transactions</li>
            <li><strong>Face Scan:</strong> Biometric authentication for secure login and withdrawals</li>
        </ul>
    </section>

    <section>
        <h2>2. Overall Description</h2>
        <h3>2.1 Product Perspective</h3>
        <p>The Digital Currency Platform will be a web-based application built using <span class="highlight">Node.js</span> for the backend, <span class="highlight">MongoDB</span> for data storage, and <span class="highlight">React.js</span> for the frontend. The mobile version will be developed using <span class="highlight">React Native</span>.</p>

        <h3>2.2 User Classes and Characteristics</h3>
        <ul>
            <li><strong>End User:</strong> Regular users who will create an account, buy coins, transfer coins, and use face scan authentication.</li>
            <li><strong>Admin:</strong> Admins who will monitor transactions, approve withdrawals, and manage users.</li>
            <li><strong>System:</strong> The platform, including its APIs, frontend, and backend components, integrated with external services like Razorpay.</li>
        </ul>

        <h3>2.3 Operating Environment</h3>
        <ul>
            <li><strong>Backend:</strong> Node.js running on a cloud-based server (e.g., Heroku, AWS)</li>
            <li><strong>Frontend:</strong> React.js for the web, React Native for the mobile app</li>
            <li><strong>Database:</strong> MongoDB hosted on a cloud service like MongoDB Atlas</li>
            <li><strong>Blockchain Simulation:</strong> Local Node.js server for simulating a blockchain</li>
        </ul>

        <h3>2.4 Constraints</h3>
        <ul>
            <li>The platform must handle a reasonable number of transactions per second, keeping in mind the simulation nature of the blockchain.</li>
            <li>Face scan authentication will be limited to devices with front-facing cameras.</li>
        </ul>
    </section>

    <section>
        <h2>3. System Features</h2>
        <h3>3.1 User Authentication</h3>
        <p><strong>Description:</strong> Users must register and log in to the platform. Authentication will be performed using JWT for session management, and passwords will be securely hashed using bcrypt.</p>
        <h3>3.2 Coin Purchase and Payment</h3>
        <p><strong>Description:</strong> Users can purchase the platform's digital currency (LaganCoin) via Razorpay.</p>
        <h3>3.3 Wallet System</h3>
        <p><strong>Description:</strong> Users will have a wallet to store their purchased coins.</p>
        <h3>3.4 Blockchain Simulation</h3>
        <p><strong>Description:</strong> A simulated blockchain will record transactions, ensuring transparency.</p>
        <h3>3.5 Face Scan Authentication</h3>
        <p><strong>Description:</strong> Users will authenticate via face scan to log in or make withdrawals.</p>
        <h3>3.6 Admin Dashboard</h3>
        <p><strong>Description:</strong> Admins will have a dashboard to monitor platform activity.</p>
    </section>

    <footer>
        <p>&copy; 2025 Digital Currency Platform</p>
    </footer>
</body>
</html>
