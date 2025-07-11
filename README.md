# Spider-Onsite-URL-Shortener-
# Building an URL Shortener with Hash Function
A lightweight URL shortening service built with **Spring Boot** techstack that:
- generates concise, unique links using a custom **hash function**
- redirects users to the original lengthy URL
- emails the shortened URL to users if they want so

---
##  Features

- Shortens long URLs using SHA-256 hashing  
- Stores URL mappings in an H2 in-memory database  
- Redirects short links to the original long URL  
- (Optional) Sends shortened URL via email  
- Simple REST API and optional web UI
---
## Tech Stack
- Java 17
- Spring Boot 3.x
- Spring Web
- Spring Data JPA
- H2 Database (for development)
- JavaMailSender (for emailing feature)
- Lombok
---

## Project Structure
src/
├── main/
│   ├── java/
│   │   └── com/thomasjayconsulting/bitlydemo/
│   │       ├── controller/         # REST API endpoints
│   │       ├── model/              # data classes including entities and request payloads 
│   │       ├── repository/         # spring data interface for dataase operatobs
│   │       ├── service/            # hashing,redirecting to shortened URL and Emailing optionally to the users
│   │       └── BitLyDemoApplication.java  # springboot class
│   │
│   └── resources/
│       ├── application.properties 
│       └── static/               
│
└── test/                       

