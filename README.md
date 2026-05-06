# exp_5
AIM:Implement user authentication and authorization features in your mobile application, allowing users to register, log in, and access personalized content.
-------------------------------------------

THEORY:
User authentication and authorization are fundamental security mechanisms used in mobile applications to ensure that only legitimate users can access the system and perform permitted actions. These mechanisms not only protect sensitive user data but also enable personalized user experiences within the application.

1. Authentication

Authentication is the process of verifying the identity of a user. It answers the question: “Who are you?” In mobile applications, authentication ensures that the user trying to access the app is genuine and matches the stored credentials.

Common authentication methods:

Username & Password
OTP (One-Time Password)
Biometric (Fingerprint/Face ID)
OAuth (Google, Facebook login)

In mobile apps, authentication is typically handled using:

Firebase Authentication
REST APIs with JWT (JSON Web Tokens)

2. Authorization

Authorization is the process of determining what an authenticated user is allowed to do. It answers the question: “What can you access?” Once a user is verified, authorization controls access to different resources and functionalities within the app.

Examples:

Admin → Full access
User → Limited access
Guest → Read-only access

3. Workflow of Authentication System
User registers (email/password stored securely)
User logs in with credentials
App verifies credentials via backend
If valid → user session/token is created
User gets access to personalized content

4. Key Features:
Secure Password Storage
Secure password handling (hashing)
Session management
Role-based access control
Logout functionality
Input Validation

5. Benefits
Data security 
Personalized experience 
Controlled access 
Prevent unauthorized usage 
-------------------------------------------
CODE:
-------------------------------------------
OUTPUT:
-------------------------------------------
LEARNING OUTCOME:
Understand how to implement user authentication and authorization to secure mobile applications.
Learn to build login, registration, and personalized user access features with proper navigation and session handling.