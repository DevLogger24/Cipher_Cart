# Cipher Cart

## Overview
Cipher Cart is a web-based marketplace for new and used electronics. The project focuses on improving how users navigate, evaluate, and compare technical products, where traditional marketplaces tend to fall short.

The system is designed as a structured, modular prototype that prioritizes clarity of data, predictable behavior, and maintainable architecture over feature breadth.

---

## Context and Motivation
Large e-commerce platforms solve discovery at scale, but introduce trade-offs in technical domains like electronics:

- Product specifications are inconsistent or poorly structured  
- Comparison across listings is difficult or unreliable  
- Search results often prioritize ranking over relevance  
- Used and refurbished products are not well integrated  

Cipher Cart explores a more structured approach where product data is consistent, comparable, and easier to reason about.

---

## Design Goals
- Deterministic and predictable system behavior  
- Clear separation of concerns across layers  
- Modular and extensible architecture  
- System usability independent of AI features  
- Consistent and structured product data  

---

## Scope

### Core
- User authentication  
- Structured product catalog  
- Filtering and search  
- Product detail views  
- Product comparison  
- Basic cart functionality  

### Experimental
- Text-based recommendations  
- Image-based similarity search  

### Out of Scope (Prototype Phase)
- Payment systems  
- Logistics/shipping  
- Large-scale seller infrastructure  
- Advanced personalization systems  

---

## System Architecture

### Presentation Layer
- Next.js frontend  
- Handles UI and user interaction  

### Application Layer
- FastAPI backend  
- Request handling and validation  

### Domain Layer
- Business logic (search, comparison, cart)  

### Data Layer
- PostgreSQL database  
- Structured and normalized schema  

### AI Module (Optional)
- Recommendation logic  
- Image similarity search  
- Isolated from core system  

---

## Key Features

### Product Catalog
- Structured categories and attributes  
- Consistent technical specifications  

### Search and Filtering
- Deterministic filtering  
- Attribute-based queries  

### Product Comparison
- Side-by-side comparison  
- Based on normalized data  

### User Management
- Authentication and sessions  

### Cart
- Basic add/remove workflow  

---

## Data Model (Conceptual)
Core entities:

- **User**  
- **Product**  
- **Category**  
- **CartItem**  

Designed to support:

- Efficient filtering  
- Structured comparison  
- Minimal redundancy  

---

## Tech Stack
- **Frontend:** Next.js (React)  
- **Backend:** FastAPI (Python)  
- **Database:** PostgreSQL  

### Rationale
- FastAPI provides a clean API layer with strong typing and validation  
- PostgreSQL supports relational integrity and complex queries required for filtering/comparison  
- Next.js allows separation of UI concerns while maintaining performance and flexibility  

---

## Project Structure
