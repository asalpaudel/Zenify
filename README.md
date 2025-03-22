# Zenify - Role based springboot ecommerce project

Welcome to **Zenify**, a modern e-commerce site for wellness and fitness built using **HTML, CSS, and the Spring framework**. 
Scroll to the Setup section to learn about installing the system to your IDE

## Features

- **User Authentication**: Secure login and registration.
- **Product Management**: Add, edit, and delete products.
- **Order Tracking**: Track the status of the order.
- **Order Processing**: View and manage orders.
- **Forgot Password**: Sends a token (reset URL) to the registered email for password reset.
- **Live Order Status Updates**: Customers receive real-time updates on their order status via email.
- **Admin Access**: Users need to toggle their role from `user` to `admin` in the database to access admin pages.

## Tech Stack

- **Frontend**: HTML, CSS
- **Backend**: Java, Spring Framework
- **Database**: MySQL 
- **Build Tool**: Maven/Gradle
- **Email Service**: Google SMTP

## Installation

### Prerequisites
- Java (JDK 17 or later)
- MySQL 
- Maven or Gradle
- Spring Boot
- Google SMTP Configuration

### Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/asalpaudel/Zenify.git
   cd Zenify
   ```
2. Configure the database in `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/zenify
   spring.datasource.username=root
   spring.datasource.password=****
   ```
3. Configure Google SMTP for email services:
   ```properties
   spring.mail.host=smtp.gmail.com
   spring.mail.port=587
   spring.mail.username=your-email@gmail.com
   spring.mail.password=your-app-password
   spring.mail.properties.mail.smtp.auth=true
   spring.mail.properties.mail.smtp.starttls.enable=true
   ```
   **Note:** To use Google SMTP, you must:
   - Add your Google email address to the code properties.
   - Enable two-step verification in your Google account.
   - Generate an **App Password** in Google and use it as the SMTP password.

4. Open your browser and visit `http://localhost:8080`

## Usage
- Register or log in as a user.
- Browse products and add them to your cart.
- Proceed to checkout and place an order.
- Receive live order status updates via email.
- If you forget your password, use the **Forgot Password** feature to reset it via email.
- To access admin features, change the user role to `admin` in the database.
- Admin users can manage products and orders.

## Contribution
We welcome contributions! Feel free to fork the repo and submit pull requests.

## Screenshots

- **Landing Page**  
  ![image](https://github.com/user-attachments/assets/221b4020-38dc-4539-9978-7e727d2f7197)

- **Login Page**  
  ![image](https://github.com/user-attachments/assets/cac811d2-0cd0-4f98-b9b3-938a1f5766f4)

- **Signup Page**  
  ![image](https://github.com/user-attachments/assets/556bfd68-6b78-4e27-b1c7-eded3af1573c)

- **Product Page**  
  ![image](https://github.com/user-attachments/assets/699594fa-4c99-43f1-b72e-4fd33b57b5f3)

- **Cart**  
  ![image](https://github.com/user-attachments/assets/d986ed59-5c2b-49e3-9651-480d0e77381f)

- **Checkout**  
  ![image](https://github.com/user-attachments/assets/5e2ad924-737f-459f-a358-abf396054027)

- **Order Successful Page**  
  ![image](https://github.com/user-attachments/assets/c168d70a-5d18-45d9-8c40-b1b02272e61a)

- **Admin Dashboard**  
  ![image](https://github.com/user-attachments/assets/9da6731f-85fb-4226-ac9b-f4e43b4ea9b5)
