# 🛒 Nexus Commerce — Backend API  
Advanced E-Commerce Backend for Project Nexus (ProDev Backend Engineering)

Nexus Commerce is a fully-featured **E-Commerce Backend API** built as the final project of the **ALX ProDev Backend Engineering Program**, demonstrating advanced backend skills, scalable architecture, and industry-standard patterns.

This project showcases real-world backend engineering practices including database modeling, REST API design, authentication, caching, background processing, documentation, and testing.

---

## 🚀 Project Overview

Nexus Commerce provides the backend infrastructure for a modern E-Commerce platform, including:

- User authentication & authorization  
- Product & category management  
- Inventory & stock control  
- Cart & checkout system  
- Orders & order items  
- Ratings & reviews  
- Caching with Redis  
- Optimized PostgreSQL database  
- Background tasks (emails, reports, notifications)  
- Comprehensive API documentation  

The project emphasizes **clean architecture**, **scalable database design**, and **professional workflows** expected from a production-grade backend system.

---

## 🏗️ Tech Stack

| Layer | Technology |
|------|------------|
| Backend Framework | Django + Django REST Framework |
| Database | PostgreSQL |
| Caching | Redis |
| Background Jobs | Celery + RabbitMQ |
| Containerization | Docker & Docker Compose |
| Authentication | JWT Authentication |
| API Documentation | Swagger / Postman Collection |
| Testing | Django Test Framework + Pytest |

---

## 🗄️ Database Design (ERD)

The Entity Relationship Diagram (ERD) models all major entities and relationships in the system, including:

- Users  
- Products  
- Categories  
- Product Variants  
- Inventory  
- Cart & Cart Items  
- Orders & Order Items  
- Reviews  

📌 **Google Doc containing the ERD:**  
👉 *[Insert your Google Doc link here]*

---

## 📦 Core Features

### 🔐 **Authentication & User Management**
- JWT-based login and registration  
- Roles & permissions (Admin / Customer)  
- Profile management  

### 🛍️ **Product & Category Management**
- CRUD operations for products  
- Hierarchical categories  
- Product variants (size, color, etc.)  
- Rich product metadata  

### 📦 **Inventory System**
- Track stock levels  
- Low-stock notifications  
- Automatic stock reduction on order placement  

### 🛒 **Cart System**
- Add/remove items  
- Update quantities  
- Cart merging  
- Automatic price calculations  

### 📑 **Orders & Checkout**
- Create orders  
- Order items  
- Payment simulation  
- Order status workflow  

### ⭐ **Reviews & Ratings**
- Post reviews for purchased products  
- Rating aggregation  

### ⚡ **Caching**
- Redis caching for:  
  - Product listing  
  - Category tree  
- Cache invalidation strategies  

### 📬 **Background Jobs**
- Sending order confirmation emails  
- Generating reports  
- Daily stock sync jobs  

---

## 📚 API Documentation

Full API documentation is provided via:

- **Swagger UI** (auto-generated)  
- **Postman Collection** (exported inside `/docs`)  

---

## 🧪 Testing

Includes:

- Unit tests for models  
- API endpoint tests  
- Integration tests (DB + API)  
- Mocking external services  

Run tests:

```bash
pytest
