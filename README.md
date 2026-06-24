# 🏨 **Bluebird — Hotel Management System (#NOT_MINE -- ReUsed & Taken From GITHUB)**

**A Complete PHP/MySQL Web Application for Hotel Reservation & Administration**

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![XAMPP](https://img.shields.io/badge/XAMPP-FB7A24?style=for-the-badge&logo=xampp&logoColor=white)

---

### 🛎️ **Book** • **Manage** • **Invoice** • **Analyze**

**Streamline hotel operations** with a full-featured web application that handles guest reservations, admin dashboard, payment processing, invoice generation, room & staff management, and real-time statistics — all following complete SDLC with UML documentation.

## 📋 **Project Overview**

Bluebird is a **comprehensive hotel management system** developed as a Software Engineering course project. It replaces manual hotel administration with an automated, centralized web application that reduces duplicate records, eliminates delayed confirmations, ensures accurate payment calculations, and provides real-time booking status tracking.

**Two Main User Roles:**
- **Guests/Users** — Register, browse rooms, submit reservations
- **Admin/Staff** — Manage bookings, confirm reservations, generate payments, print invoices, manage rooms & staff, view dashboard statistics

**Complete SDLC Coverage:**
- ✅ Requirements Analysis (Elicitation, Scope, SMART, MoSCoW)
- ✅ Specification (SRS, Use Cases, Traceability Matrix)
- ✅ Design (Architecture, Database, UML Diagrams)
- ✅ Implementation (PHP, MySQL, Bootstrap, JavaScript)
- ✅ Testing (14 Test Cases, All Verified)
- ✅ Maintenance (Corrective, Adaptive, Perfective, Preventive)
- ✅ Retirement Planning

## 🚀 **Key Features**

| Feature | Description | Icon |
|---------|-------------|------|
| **👤 User Registration & Login** | Secure account creation and authentication | 👤 |
| **🏨 Room Browsing** | View hotel facilities and available room types | 🏨 |
| **📝 Online Booking** | Submit reservation with guest info, dates, meal plans | 📝 |
| **✅ Admin Booking Confirmation** | Review and confirm pending reservations | ✅ |
| **💰 Auto Payment Calculation** | Room rent + bed rent + meals × days = total | 💰 |
| **🧾 Printable Invoices** | Professional invoice generation with hotel branding | 🧾 |
| **🛏️ Room Management** | Add/delete room records (type, bedding) | 🛏️ |
| **👥 Staff Management** | Add/delete staff records (name, role) | 👥 |
| **📊 Dashboard Statistics** | Real-time counts: bookings, rooms, staff, profit | 📊 |
| **📤 Data Export** | Export booking data for reporting | 📤 |
| **🔒 Session-Based Security** | Role-based access control for admin pages | 🔒 |
| **📱 Responsive Design** | Bootstrap-powered mobile-friendly interface | 📱 |

## 🛠️ **Tech Stack**

| Layer | Technology | Purpose |
|-------|------------|---------|
| **Backend** | PHP | Server-side logic, session handling, database queries |
| **Database** | MySQL / MariaDB | Persistent data storage (`bluebirdhotel`) |
| **Frontend** | HTML5, CSS3, Bootstrap 5 | Responsive UI components and layout |
| **Client-Side** | JavaScript | Form validation, table search, page interactions |
| **Server** | Apache (XAMPP) | Local web server environment |
| **Tools** | phpMyAdmin, Draw.io/StarUML | Database management & UML modeling |

## 📁 **Project Structure**

```bash
bluebird-hotel-management/
├── index.php                     # Main entry: user login, signup, admin login
├── home.php                      # User homepage with room browsing & booking form
├── config.php                    # Database connection settings
├── logout.php                    # Session termination
├── admin/
│   ├── admin.php                 # Admin layout with dashboard frame
│   ├── dashboard.php             # Statistics cards & charts
│   ├── roombook.php              # Booking management (view, confirm, delete)
│   ├── roomconfirm.php           # Booking confirmation & payment insertion
│   ├── payment.php               # Payment records table & search
│   ├── invoiceprint.php          # Printable invoice page
│   ├── room.php                  # Room add/delete management
│   ├── staff.php                 # Staff add/delete management
│   └── assets/                   # Admin CSS, JS, images
├── css/
│   ├── home.css                  # Homepage custom styles
│   └── login.css                 # Login page custom styles
├── javascript/
│   └── index.js                  # Client-side interactions
├── image/                        # Hotel photos & room images
├── photos/                       # Additional media assets
├── bluebirdhotel.sql             # Complete database schema + sample data
└── README.md                     # This file
```

## 🖥️ **Installation & Quick Start**

### Prerequisites
- XAMPP (Apache + MySQL + PHP)
- Modern web browser (Chrome, Edge, Firefox)

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/bluebird-hotel-management.git
cd bluebird-hotel-management
```

### 2. Move to XAMPP htdocs
```bash
# Windows
move bluebird-hotel-management C:\xampp\htdocs\

# Or manually copy the project folder to C:\xampp\htdocs\
```

### 3. Create Database
1. Start **XAMPP Control Panel** → Start **Apache** and **MySQL**
2. Open browser → `http://localhost/phpmyadmin`
3. Click **New** → Create database named `bluebirdhotel`
4. Select `bluebirdhotel` → Click **Import** tab
5. Choose `bluebirdhotel.sql` from project folder → Click **Go**

### 4. Configure Database Connection
Edit `config.php`:
```php
$servername = "localhost";
$username = "root";
$password = "";          # Default XAMPP has no password
$database = "bluebirdhotel";
```

### 5. Launch Application
```
http://localhost/bluebird-hotel-management/index.php
```

### 6. Test Accounts

| Role | Email | Password |
|------|-------|----------|
| **Admin/Staff** | `admin@gmail.com` | `1234` |
| **User** | `test@gmail.com` | `123` |
| **User** | `mohamed@gmail.com` | `mohamed@gmail.com` |

## 🎮 **How to Use**

### Guest/User Flow
```
1. Open homepage → Browse rooms & facilities
2. Click "Book" → Login or Sign up
3. Fill reservation form (name, email, country, phone)
4. Select room type, bed type, meal plan, dates
5. Submit → Booking saved as "NotConfirm"
6. Wait for admin confirmation
```

### Admin/Staff Flow
```
1. Login with admin credentials
2. Dashboard → View statistics (bookings, rooms, staff, profit)
3. Room Booking → View all reservations → Click "Confirm"
4. Payment → Auto-calculated totals appear → Print Invoice
5. Rooms → Add new room types or delete existing
6. Staff → Add new employees or remove records
```

### Booking Confirmation & Payment
```
Admin clicks "Confirm" on a booking → System:
├── Updates status: NotConfirm → Confirm
├── Calculates: Room Rent + Bed Rent + (Meals × Days)
├── Creates payment record in database
└── Enables "Print Invoice" button
```

## 📊 **Database Schema**

### Tables

| Table | Purpose | Key Columns |
|-------|---------|-------------|
| **signup** | User accounts | UserID, Username, Email, Password |
| **emp_login** | Admin/staff accounts | empid, Emp_Email, Emp_Password |
| **room** | Available room types | id, type, bedding |
| **roombook** | Reservation records | id, Name, Email, Country, Phone, RoomType, Bed, Meal, NoofRoom, cin, cout, nodays, stat |
| **payment** | Payment records | id, Name, Email, RoomType, Bed, NoofRoom, cin, cout, nodays, roomtotal, bedtotal, mealtotal, finaltotal |
| **staff** | Employee records | id, name, work |

### Entity Relationships
```
User ──creates──► Booking ──generates──► Payment ──printed as──► Invoice
                                    │
Admin ──manages──► Room, Staff, Booking, Payment
```

## 📐 **UML Diagrams**

The project includes comprehensive UML documentation:

| Diagram | Description | Status |
|---------|-------------|--------|
| **Use Case Diagram** | Guest & Admin interactions with the system | ✅ |
| **Class Diagram** | Entity classes: User, Room, Booking, Payment, Staff, Admin | ✅ |
| **Sequence Diagram** | Booking flow: Guest → UI → Controller → Payment → Database | ✅ |
| **Activity Diagram** | Guest booking process from homepage to confirmation | ✅ |
| **State Diagram** | Booking lifecycle: Homepage → Browse → Login → Book → Confirm | ✅ |
| **Package Diagram** | Code organization: Public, Admin, Shared Assets, Config | ✅ |
| **Component Diagram** | System components: Frontend, Booking, Payment, Staff, Database | ✅ |
| **Collaboration Diagram** | Object interactions during booking process | ✅ |

## ✅ **Testing Results**

All 14 test cases verified:

| Test ID | Scenario | Status |
|---------|----------|--------|
| TC-01 | User signup | ✅ Verified |
| TC-02 | User login | ✅ Verified |
| TC-03 | Admin login | ✅ Verified |
| TC-04 | Submit booking | ✅ Verified |
| TC-05 | View bookings | ✅ Verified |
| TC-06 | Confirm booking | ✅ Verified |
| TC-07 | Generate payment | ✅ Verified |
| TC-08 | Print invoice | ✅ Verified |
| TC-09 | Add room | ✅ Verified |
| TC-10 | Delete room | ✅ Verified |
| TC-11 | Add staff | ✅ Verified |
| TC-12 | Delete staff | ✅ Verified |
| TC-13 | Dashboard statistics | ✅ Verified |
| TC-14 | Invalid login | ✅ Verified |

## 🔒 **Security Features**

- **Session Management** — PHP sessions distinguish logged-in users/admins
- **Admin Page Protection** — Direct access blocked without valid session
- **Input Validation** — Basic required-field checks on all forms
- **SQL Injection Prevention** — Partial prepared statements (recommended: convert all)
- **Password Security** — Future improvement: `password_hash()` + `password_verify()`

## 🔮 **Future Improvements**

- 🔐 **Password Hashing** — Replace plain text with bcrypt hashing
- 🛡️ **Prepared Statements** — Convert all direct SQL to parameterized queries
- 📅 **Date Validation** — Stricter checks for check-in/check-out dates
- 📧 **Email/SMS Notifications** — Automated booking confirmations
- 💳 **Online Payment Gateway** — Stripe/PayPal integration
- 📱 **Mobile App** — Companion iOS/Android application
- 📊 **Advanced Reports** — Monthly/yearly financial analytics
- 🏨 **Multi-Branch Support** — Chain hotel management
- 🔍 **Room Availability Calendar** — Visual booking calendar
- 🌐 **Live Deployment** — Cloud hosting with SSL

## 🧠 **Software Engineering Concepts Covered**

- **SDLC Phases** — Complete lifecycle from requirements to retirement
- **Requirements Elicitation** — Prototyping, observation, interviews, workshops
- **SMART Requirements** — Specific, Measurable, Achievable, Relevant, Time-based
- **MoSCoW Prioritization** — Must/Should/Could/Won't-Have classification
- **SRS Documentation** — Formal specification with traceability matrix
- **UML Modeling** — 8 diagram types for design documentation
- **3-Tier Architecture** — Presentation, Application, Data layers
- **Modular Design** — Separation of concerns across files
- **Testing Strategy** — Desk checking, unit, integration, system, acceptance, regression
- **Maintenance Planning** — Corrective, adaptive, perfective, preventive strategies

## 👥 **Team**

| # | Name | ID |
|---|------|-----|
| 1 | Hossam Ahmed Adel | 2305037 |
| 2 | Antony Medhat Makram | 2305065 |
| 3 | Mohamed Ibrahim Hussein | 2305026 |
| 4 | Youssef Ahmed Wahid | 2305105 |
| 5 | Mayer Adel Kher | 2305083 |

**Institution:** Faculty of Computer & Data Science, Alexandria National University, Alexandria, Egypt

**Course:** Software Engineering

## 📜 **License**

This project is licensed under the **MIT License** — free to use for education, research, and commercial purposes.

---

⭐ **Star this repo if you found it helpful for learning software engineering!**
