# CS F213 - Book Exchange Portal  
## A Simple Web App for Borrowing and Sharing Books

This is a **Book Exchange Portal**, built as part of the **CS F213 - Object-Oriented Programming** course. It’s basically a **book-sharing system** where users can **list books they own, request books from others, and manage exchanges easily**. The platform also comes with **user accounts, admin controls, and a transaction system** to keep everything organized.

---

## What This Project Does
This web app makes **borrowing and lending books** super easy. Here’s what you can do:

### **For Regular Users**
- **Sign up & log in** – Create an account and access the system securely.
- **Manage your profile** – Update personal details when needed.
- **List books for exchange** – Add books you want to lend.
- **Request books** – Browse available books and send borrow requests.
- **Approve or reject requests** – Decide who can borrow your books.
- **Search for books or users** – Find books based on title or owner.
- **Change your password** – Keep your account secure.

### **For Admins**
- **Manage users** – Create, disable, or delete accounts if needed.
- **Monitor transactions** – Keep an eye on book exchanges.
- **Resolve disputes** – Step in when users have issues.

---

## How to Run This Project

### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/BookExchangePortal.git
cd BookExchangePortal-main
```

### **2. Set Up the Database**
- Create a **MySQL or PostgreSQL** database.
- Run the provided **schema.sql** file to set up tables.
- Update **ConnectionProvider.java** with your database details.

### **3. Start the Application**
If you're using **Apache Tomcat**, deploy the project by:
1. Placing the `BookExchangePortal` folder inside the `webapps/` directory.
2. Starting the Tomcat server.
3. Opening a browser and going to:
http://localhost:8080/BookExchangePortal

If you prefer running it manually:
```bash
javac -d build/classes src/main/java/com/my/**/*.java
java -cp build/classes com.my.servlet.LoginServlet
```
---

## How the Book Exchange Process Works
1. **User signs up and logs in** – New users register and existing users log in securely.
2. **User lists books they are willing to share** – Users can add books to their inventory.
3. **Other users browse available books** – The system allows searching and filtering.
4. **A user sends a request to borrow a book** – The book owner gets notified.
5. **Book owner can accept or reject the request** – Once approved, the book is considered borrowed.
6. **After borrowing, the book is marked as in use** – The system keeps track of active exchanges.
7. **Once the book is returned, the transaction is completed** – Admins can oversee disputes if needed.

---

## Technologies Used
- **Java (JSP & Servlets)** – Handles backend logic.
- **JSP (JavaServer Pages)** – Renders dynamic HTML content.
- **MySQL / PostgreSQL** – Stores user and book data.
- **HTML, CSS, JavaScript** – Enhances frontend functionality.
- **Apache Tomcat** – Runs the web application.

---

## Future Improvements
The system works well, but there are several ways it could be even better:
- **Book Ratings & Reviews** – Let users rate books after borrowing.
- **Email Notifications** – Notify users when a book request is approved or rejected.
- **Book Recommendation System** – Suggest books based on borrowing history.
- **Mobile-Friendly UI** – Improve layout for better usability on phones and tablets.

---
