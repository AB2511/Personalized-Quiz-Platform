# Personalized Quiz Platform

## 🎮 **Overview**

The **Personalized Quiz Platform** is an interactive web application built by us a group of college students. The platform allows users to **register**, **login**, and play quizzes on various topics. Users can customize their quiz experience by selecting the **number of questions**, **difficulty level**, and the **field** of the questions. Each question comes with a fixed **60-second timer**, making it both fun and challenging. After completing the quiz, users can see their scores, retake the quiz, or return to the welcome page.

### **Key Features:**
- **User Registration & Login**: Secure user authentication system.
- **Customizable Quizzes**: Choose the **number of questions**, **difficulty level**, and **topic**.
- **60-Second Timer**: Each question comes with a countdown timer to make the quiz more engaging.
- **Dynamic Questions**: Questions are fetched from an API for a unique quiz experience every time.
- **Score Display**: Scores are shown at the end of the game.
- **Retake Quiz or Logout**: Users can retake the quiz or return to the welcome page.

---

## 🔧 **Tech Stack**

- **Backend**: Java, Servlets
- **Frontend**: HTML, CSS, JavaScript
- **Database**: MySQL
- **Libraries/Tools**: MySQL Connector for Java, Eclipse IDE, Apache Tomcat

---

## ⚙️ **How to Run the Project Locally**

### 1. **Clone the Repository**

Clone the repository to your local machine using the following command:

```bash
git clone https://github.com/AB2511/Personalized-Quiz-Platform.git
```

### 2. **Set Up the Database**
1. Install **MySQL** and set up a new database.
2. Use the provided `database.sql` file to set up the database schema:
   
```sql
-- Example SQL setup (check database.sql for details)
CREATE DATABASE quiz_platform;
USE quiz_platform;
-- Import tables and data
```

### 3. **Configure the Database Connection**
- Open the `DBUtil.java` file and update the database connection details:
  - **Database URL**
  - **Username**
  - **Password**
  
Ensure the database is running and the connection details are correct.

### 4. **Run the Application**
1. Open the project in **Eclipse IDE** (or any Java IDE that supports Servlets).
2. Deploy the application to a local **Apache Tomcat** server (or any Servlet container).
3. Visit `http://localhost:8080/` to start using the platform.

### 5. **User Flow**
- **Register** on the homepage (`index.html`).
- After successful registration, **login** through the login page (`login.jsp`).
- Upon successful login, users are directed to a **welcome page** where they can:
  - Start the quiz by selecting the **number of questions**, **difficulty**, and **category**.
  - Log out to return to the login page.

---

## 📝 **Project Structure**

```
Personalized-Quiz-Platform/
├── src/                           # Java source files
│   ├── com/quizapp/
│   │   ├── controller/             # Handles user requests and serves dynamic content
│   │   │   ├── LoginsServlet.java  # Handles user login requests
│   │   │   ├── RegistersServlet.java # Handles user registration requests
│   │   ├── dao/                   # Data Access Objects for database operations
│   │   │   ├── UserDao.java        # Interface for user operations
│   │   │   ├── UserDaoImpl.java    # Implementation of user database operations
│   │   └── model/                 # Model classes (User.java)
├── webapp/                        # Web application files
│   ├── index.html                 # Home page for login/signup
│   ├── login.jsp                  # Login page (JSP)
│   ├── logout.jsp                 # Logout page (JSP)
│   ├── register.jsp               # User registration page (JSP)
│   ├── welcome.jsp                # Welcome page after login
│   ├── quiz.jsp                   # Quiz page where users can select quiz settings
│   ├── result.jsp                 # Results page displaying the user's score
│   ├── styles.css                 # Global styles for the platform
│   └── script.js                  # JavaScript for handling quiz interaction
├── resources/                     # Additional resources (e.g., logos, images)
│   ├── websitelogo.png            # Logo for the website
│   ├── contactusat.png            # Contact image
└── libs/                          # External libraries
    └── mysql-connector-java-8.0.28.jar  # MySQL JDBC connector
```

---


### **Enjoy the Quiz!** 🎉

---
