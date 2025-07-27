# Atm-Simulator

An intuitive and fully functional **ATM Simulator** built with **Java Swing**. This project replicates the core banking functionalities of an Automated Teller Machine, including user authentication, balance enquiry, deposit, withdrawal, PIN change, and more. Designed with a step-by-step sign-up flow and image-enhanced GUI for an engaging experience.


## 🛠️ Features

- User Signup and Login (3-step form)
- Deposit and Withdraw money
- Fast cash withdrawal with fixed amounts
- Balance enquiry
- View mini statement (transaction history)
- PIN change functionality


## 📁 Project Structure

ATM-Simulator/
├── src/
│ ├── javacodes/
│ │ ├── SignUp.java
│ │ ├── SignUp2.java
│ │ ├── SignUp3.java
│ │ ├── Login.java
│ │ ├── Deposit.java
│ │ ├── Withdrawal.java
│ │ ├── FastCash.java
│ │ ├── BalanceEnquiry.java
│ │ ├── MiniStatement.java
│ │ ├── PinChange.java
│ │ └── Transaction.java
│ └── images/
│ | ├── atm.jpg
│ | ├── logo.jpg
│ | └── atmdashboard.jpg
└── README.md



## 🛠️ Technologies Used

* **Java 8 or higher**
* **Java Swing** – for designing the graphical user interface (GUI)
* **AWT (Abstract Window Toolkit)** – for layout managers and event handling
* **JDBC (Java Database Connectivity)** – to connect Java with MySQL database
* **MySQL** – for storing user and transaction data
* **JCalendar Library** – used for date picking in forms
* **File I/O** – for potential data handling and logging
* **Eclipse IDE** – preferred development environment (can use IntelliJ or VS Code with Java extensions)



## 🔧 How to Run the Project

### ✅ Prerequisites

Make sure the following tools and files are set up before running the project:

* Java JDK 8 or above installed
* Eclipse IDE or compatible Java IDE (like IntelliJ or VS Code)
* MySQL Server installed
* MySQL Connector JAR (mysql-connector-j-9.1.0.jar) added to the project's build path
* JCalendar JAR (jcalendar.jar) added to the project’s build path
* Database named **bank management system** created in MySQL (with the required tables)



## ▶️ Run Steps

1. **Open Eclipse IDE**

2. **Import Project:**

   * Go to `File → Import → Existing Projects into Workspace`
   * Select the folder where the project (`ATM-Simulator`) is located
3. **Configure Build Path:**

   * Right-click on the project → `Build Path → Configure Build Path`
   * Add External JARs:

     * `mysql-connector-j-9.1.0.jar`
     * `jcalendar.jar`
4. **Setup Database:**

   * Open MySQL
   * Create a database:

     ```sql
     CREATE DATABASE `bank management system`;
     ```
   * Execute the provided `.sql` file (in the zip) to create necessary tables like `login`, `signup`, `bank`, etc.
5. **Run the Project:**

   * Start with the file: `Signup.java` (for new users) or `Login.java` (if credentials exist)
   * You can also test transaction screens like `Deposit.java`, `Withdrawl.java`, `BalanceEnquiry.java`, etc.
6. **Use the GUI:**

   * Perform banking operations via the ATM-style interface.



## 📚 Functional Flow

    A[SignUp Page 1] --> B[SignUp Page 2];
    B --> C[SignUp Page 3];
    C --> D[Login Page];
    D --> E[Transaction Menu];
    E --> F[Deposit];
    E --> G[Withdraw];
    E --> H[Fast Cash];
    E --> I[PIN Change];
    E --> J[Balance Enquiry];
    E --> K[Mini Statement];
