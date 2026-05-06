# Experiment 5: User Authentication & Authorization

## AIM
Implement user authentication and authorization features in a mobile application, allowing users to register, log in, and access personalized content.

---

## THEORY

User authentication and authorization are fundamental security mechanisms used in mobile applications to ensure that only legitimate users can access the system and perform permitted actions. These mechanisms not only protect sensitive user data but also enable a personalized user experience.

### 1. Authentication

Authentication is the process of verifying the identity of a user. It answers the question:  
**"Who are you?"**

In mobile applications, authentication ensures that the user accessing the app is genuine and matches the stored credentials.

#### Common Authentication Methods:
- Username & Password  
- OTP (One-Time Password)  
- Biometric Authentication (Fingerprint / Face ID)  
- OAuth (Google, Facebook Login)

#### Technologies Used:
- Firebase Authentication  
- REST APIs with JWT (JSON Web Tokens)

---

### 2. Authorization

Authorization determines what an authenticated user is allowed to do. It answers the question:  
**"What can you access?"**

After successful authentication, authorization controls access to various features and resources.

#### Examples:
- **Admin:** Full access  
- **User:** Limited access  
- **Guest:** Read-only access  

---

### 3. Authentication Workflow

1. User registers with email and password  
2. Credentials are securely stored (hashed)  
3. User logs in with credentials  
4. App verifies credentials via backend  
5. If valid → session/token is generated  
6. User gains access to personalized content  

---

### 4. Key Features

- Secure password storage (hashing)  
- Session management  
- Role-based access control (RBAC)  
- Logout functionality  
- Input validation  

---

### 5. Benefits

- Data security  
- Personalized user experience  
- Controlled access  
- Prevention of unauthorized usage  

---

## CODE

```java
// Example: Firebase Login Snippet
mAuth.signInWithEmailAndPassword(email, password)
    .addOnCompleteListener(task -> {
        if (task.isSuccessful()) {
            // Login success
        } else {
            // Login failed
        }
    });