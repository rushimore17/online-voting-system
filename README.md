# online-voting-system
The  system aims to replace the traditional paper-based voting process with a secure, transparent, and  efficient web-based platform that allows registered users to cast their votes electronically. 

https://yadnyeshkolte.github.io/online-voting-system/

This document provides a reference for the RESTful API endpoints available in the Online Voting System. The API is divided into public (Authentication, Verification) and protected (Admin, User) sections.

## Authentication & Verification
Base URL: `/api/auth`

| Method | Endpoint | Description | Request Body |
| :--- | :--- | :--- | :--- |
| `POST` | `/login` | Authenticate a user or admin. | `LoginRequest` (email, password) |
| `POST` | `/register` | Register a new user (requires identity verification). | `RegisterRequest` (details + Aadhar/VoterID) |
