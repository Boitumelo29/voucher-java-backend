# 🎟️ Voucher Java Backend

A Spring Boot backend for generating and redeeming unique 10-digit voucher codes that can be linked to a user account. This backend powers voucher flows for web or mobile applications (e.g. Flutter frontend).

---

## 🚀 Features

- ✅ Generate 10-digit numeric vouchers with fixed R-value
- ✅ Store vouchers in H2 in-memory database
- ✅ Redeem vouchers by code and associate with a user
- ✅ Prevent duplicate redemptions
- ✅ Track voucher history by user ID
- ✅ RESTful API with simple endpoints

---

## 🛠️ Tech Stack

- Java 17+
- Spring Boot 3
- Spring Data JPA
- H2 Database (dev mode)
- Maven

---

## 📦 Installation

### Prerequisites
- JDK 17+
- Maven
- IntelliJ / VS Code / Terminal




Run the App
./mvnw spring-boot:run


🔌 API Endpoints
🧾 Generate Voucher
POST /api/vouchers/generate?amount=60
Response:
{
  "code": "1234567890",
  "amount": 60,
  "redeemed": false,
  "redeemedBy": null
}

