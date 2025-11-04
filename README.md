# 💳 POS (Point of Sale) System

A full-stack **Point of Sale (POS)** web application designed to automate billing, inventory management, customer tracking, and reporting for retail businesses.  
Built using **React.JS** (frontend) and **Spring Boot** (backend), it provides real-time analytics, secure authentication, and subscription-based multi-store management.

---

## 🧭 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [System Architecture](#-system-architecture)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Project Structure](#-project-structure)
- [API Overview](#-api-overview)
- [Screenshots](#-screenshots)
- [Testing](#-testing)
- [Future Enhancements](#-future-enhancements)
- [Contributors](#-contributors)
- [License](#-license)

---

## 🚀 Overview

The **POS System** helps businesses streamline store operations through:

- Fast and error-free billing
- Real-time stock and inventory tracking
- Customer management and order history
- Advanced analytics dashboards
- Centralized control for multiple stores via a Super Admin module

This system is scalable, secure, and optimized for modern retail workflows.

---

## ✨ Features

### 🛒 POS & Billing

- Product search and quick checkout
- Discount, tax, and refund support
- Auto invoice generation

### 📦 Inventory Management

- Real-time stock tracking
- Low-stock alerts and product categorization

### 👥 Customer Management

- Add and update customer details
- View complete order and billing history

### 🧑‍💼 Admin Panel

- Manage users, roles, and access
- Super Admin can handle multiple stores and subscriptions

### 💰 Payment Integration

- Supports **Razorpay** and **Stripe**
- Secure transactions with confirmation emails

### 📊 Reports & Analytics

- Sales charts, shift summaries, and store comparisons
- Exportable reports (PDF/CSV)

---

## 🏗️ System Architecture

```

Frontend (React)
↓
REST API (Spring Boot)
↓
Business Logic Layer (Spring Services)
↓
Database (MySQL)
↓
Analytics & Reporting Layer

```

---

## 💻 Tech Stack

| Layer               | Technology                                    |
| ------------------- | --------------------------------------------- |
| **Frontend**        | React.js, Tailwind CSS / Bootstrap            |
| **Backend**         | Spring Boot, Spring Security, Spring Data JPA |
| **Database**        | MySQL                                         |
| **Authentication**  | JWT (JSON Web Token)                          |
| **Payments**        | Razorpay, Stripe                              |
| **Testing**         | JUnit, Mockito                                |
| **Build Tools**     | Maven                                         |
| **Version Control** | Git, GitHub                                   |

---

---

## 📁 Project Structure

# File Tree: Full-Stack Java POS MS

**Generated:** 11/4/2025, 9:45:27 PM
**Root Path:** `e:\My Projects\SaaS POS System Using Java Full-Stack Retail & Supermarkets\Source Code & Docs\Full-Stack Java POS MS`

```
├── 📁 pos-backend
│   ├── 📁 .mvn
│   │   └── 📁 wrapper
│   │       └── 📄 maven-wrapper.properties
│   ├── 📁 src
│   │   ├── 📁 main
│   │   │   ├── 📁 java
│   │   │   │   └── 📁 com
│   │   │   │       └── 📁 zosh
│   │   │   │           ├── 📁 configrations
│   │   │   │           │   ├── ☕ AppConfig.java
│   │   │   │           │   ├── ☕ CustomAuthenticationEntryPoint.java
│   │   │   │           │   ├── ☕ EmailUtil.java
│   │   │   │           │   ├── ☕ JwtConstant.java
│   │   │   │           │   ├── ☕ JwtProvider.java
│   │   │   │           │   ├── ☕ JwtValidator.java
│   │   │   │           │   └── ☕ SecurityConfig.java
│   │   │   │           ├── 📁 controller
│   │   │   │           │   ├── ☕ AdminDashboardController.java
│   │   │   │           │   ├── ☕ AuthController.java
│   │   │   │           │   ├── ☕ BranchAnalyticsController.java
│   │   │   │           │   ├── ☕ BranchController.java
│   │   │   │           │   ├── ☕ CategoryController.java
│   │   │   │           │   ├── ☕ CustomerController.java
│   │   │   │           │   ├── ☕ EmployeeController.java
│   │   │   │           │   ├── ☕ HomeController.java
│   │   │   │           │   ├── ☕ InventoryController.java
│   │   │   │           │   ├── ☕ OrderController.java
│   │   │   │           │   ├── ☕ PaymentController.java
│   │   │   │           │   ├── ☕ ProductController.java
│   │   │   │           │   ├── ☕ RefundController.java
│   │   │   │           │   ├── ☕ ShiftReportController.java
│   │   │   │           │   ├── ☕ StoreAnalyticsController.java
│   │   │   │           │   ├── ☕ StoreController.java
│   │   │   │           │   ├── ☕ SubscriptionController.java
│   │   │   │           │   ├── ☕ SubscriptionPlanController.java
│   │   │   │           │   └── ☕ UserController.java
│   │   │   │           ├── 📁 domain
│   │   │   │           │   ├── ☕ BillingCycle.java
│   │   │   │           │   ├── ☕ InternalCodeEnum.java
│   │   │   │           │   ├── ☕ OrderStatus.java
│   │   │   │           │   ├── ☕ PaymentMethod.java
│   │   │   │           │   ├── ☕ PaymentOrderStatus.java
│   │   │   │           │   ├── ☕ PaymentStatus.java
│   │   │   │           │   ├── ☕ PaymentType.java
│   │   │   │           │   ├── ☕ StoreStatus.java
│   │   │   │           │   ├── ☕ SubscriptionStatus.java
│   │   │   │           │   └── ☕ UserRole.java
│   │   │   │           ├── 📁 exception
│   │   │   │           │   ├── ☕ AccessDeniedException.java
│   │   │   │           │   ├── ☕ GlobalExceptionHandler.java
│   │   │   │           │   ├── ☕ ResourceNotFoundException.java
│   │   │   │           │   └── ☕ UserException.java
│   │   │   │           ├── 📁 mapper
│   │   │   │           │   ├── ☕ AuthResponseMapper.java
│   │   │   │           │   ├── ☕ BranchMapper.java
│   │   │   │           │   ├── ☕ CategoryMapper.java
│   │   │   │           │   ├── ☕ InventoryMapper.java
│   │   │   │           │   ├── ☕ OrderItemMapper.java
│   │   │   │           │   ├── ☕ OrderMapper.java
│   │   │   │           │   ├── ☕ ProductMapper.java
│   │   │   │           │   ├── ☕ RefundMapper.java
│   │   │   │           │   ├── ☕ ShiftReportMapper.java
│   │   │   │           │   ├── ☕ StoreMapper.java
│   │   │   │           │   ├── ☕ SubscriptionMapper.java
│   │   │   │           │   └── ☕ UserMapper.java
│   │   │   │           ├── 📁 messaging
│   │   │   │           ├── 📁 modal
│   │   │   │           │   ├── ☕ Branch.java
│   │   │   │           │   ├── ☕ Category.java
│   │   │   │           │   ├── ☕ Customer.java
│   │   │   │           │   ├── ☕ Inventory.java
│   │   │   │           │   ├── ☕ Order.java
│   │   │   │           │   ├── ☕ OrderItem.java
│   │   │   │           │   ├── ☕ PasswordResetToken.java
│   │   │   │           │   ├── ☕ PaymentOrder.java
│   │   │   │           │   ├── ☕ PaymentSummary.java
│   │   │   │           │   ├── ☕ Product.java
│   │   │   │           │   ├── ☕ Refund.java
│   │   │   │           │   ├── ☕ ShiftReport.java
│   │   │   │           │   ├── ☕ Store.java
│   │   │   │           │   ├── ☕ StoreContact.java
│   │   │   │           │   ├── ☕ Subscription.java
│   │   │   │           │   ├── ☕ SubscriptionPlan.java
│   │   │   │           │   └── ☕ User.java
│   │   │   │           ├── 📁 payload
│   │   │   │           │   ├── 📁 AdminAnalysis
│   │   │   │           │   │   ├── ☕ DashboardSummaryDTO.java
│   │   │   │           │   │   ├── ☕ StoreRegistrationStatDTO.java
│   │   │   │           │   │   └── ☕ StoreStatusDistributionDTO.java
│   │   │   │           │   ├── 📁 StoreAnalysis
│   │   │   │           │   │   ├── ☕ BranchPerformanceDTO.java
│   │   │   │           │   │   ├── ☕ BranchSalesDTO.java
│   │   │   │           │   │   ├── ☕ CategorySalesDTO.java
│   │   │   │           │   │   ├── ☕ PaymentInsightDTO.java
│   │   │   │           │   │   ├── ☕ StoreAlertDTO.java
│   │   │   │           │   │   ├── ☕ StoreOverviewDTO.java
│   │   │   │           │   │   ├── ☕ TimeSeriesDataDTO.java
│   │   │   │           │   │   └── ☕ TimeSeriesPointDTO.java
│   │   │   │           │   ├── 📁 dto
│   │   │   │           │   │   ├── ☕ BranchDTO.java
│   │   │   │           │   │   ├── ☕ BranchDashboardOverviewDTO.java
│   │   │   │           │   │   ├── ☕ CashierPerformanceDTO.java
│   │   │   │           │   │   ├── ☕ CategoryDTO.java
│   │   │   │           │   │   ├── ☕ CategorySalesDTO.java
│   │   │   │           │   │   ├── ☕ DailySalesDTO.java
│   │   │   │           │   │   ├── ☕ InventoryDTO.java
│   │   │   │           │   │   ├── ☕ OrderDTO.java
│   │   │   │           │   │   ├── ☕ OrderItemDTO.java
│   │   │   │           │   │   ├── ☕ ProductDTO.java
│   │   │   │           │   │   ├── ☕ ProductPerformanceDTO.java
│   │   │   │           │   │   ├── ☕ RefundDTO.java
│   │   │   │           │   │   ├── ☕ ShiftReportDTO.java
│   │   │   │           │   │   ├── ☕ StoreDTO.java
│   │   │   │           │   │   ├── ☕ SubscriptionDTO.java
│   │   │   │           │   │   └── ☕ UserDTO.java
│   │   │   │           │   ├── 📁 request
│   │   │   │           │   │   ├── ☕ ForgotPasswordRequest.java
│   │   │   │           │   │   ├── ☕ LoginDto.java
│   │   │   │           │   │   └── ☕ ResetPasswordRequest.java
│   │   │   │           │   └── 📁 response
│   │   │   │           │       ├── ☕ ApiResponse.java
│   │   │   │           │       ├── ☕ ApiResponseBody.java
│   │   │   │           │       ├── ☕ AuthResponse.java
│   │   │   │           │       ├── ☕ ExceptionResponse.java
│   │   │   │           │       └── ☕ PaymentLinkResponse.java
│   │   │   │           ├── 📁 repository
│   │   │   │           │   ├── ☕ BranchRepository.java
│   │   │   │           │   ├── ☕ CategoryRepository.java
│   │   │   │           │   ├── ☕ CustomerRepository.java
│   │   │   │           │   ├── ☕ InventoryRepository.java
│   │   │   │           │   ├── ☕ OrderItemRepository.java
│   │   │   │           │   ├── ☕ OrderRepository.java
│   │   │   │           │   ├── ☕ PasswordResetTokenRepository.java
│   │   │   │           │   ├── ☕ PaymentOrderRepository.java
│   │   │   │           │   ├── ☕ ProductRepository.java
│   │   │   │           │   ├── ☕ RefundRepository.java
│   │   │   │           │   ├── ☕ ShiftReportRepository.java
│   │   │   │           │   ├── ☕ StoreRepository.java
│   │   │   │           │   ├── ☕ SubscriptionPlanRepository.java
│   │   │   │           │   ├── ☕ SubscriptionRepository.java
│   │   │   │           │   └── ☕ UserRepository.java
│   │   │   │           ├── 📁 service
│   │   │   │           │   ├── 📁 impl
│   │   │   │           │   │   ├── ☕ AdminDashboardServiceImpl.java
│   │   │   │           │   │   ├── ☕ AuthServiceImpl.java
│   │   │   │           │   │   ├── ☕ BranchAnalyticsServiceImpl.java
│   │   │   │           │   │   ├── ☕ BranchServiceImpl.java
│   │   │   │           │   │   ├── ☕ CategoryServiceImpl.java
│   │   │   │           │   │   ├── ☕ CustomUserImplementation.java
│   │   │   │           │   │   ├── ☕ CustomerServiceImpl.java
│   │   │   │           │   │   ├── ☕ DataInitializationComponent.java
│   │   │   │           │   │   ├── ☕ EmailServiceImpl.java
│   │   │   │           │   │   ├── ☕ EmployeeServiceImpl.java
│   │   │   │           │   │   ├── ☕ InventoryServiceImpl.java
│   │   │   │           │   │   ├── ☕ OrderServiceImpl.java
│   │   │   │           │   │   ├── ☕ PaymentServiceImpl.java
│   │   │   │           │   │   ├── ☕ ProductServiceImpl.java
│   │   │   │           │   │   ├── ☕ RefundServiceImpl.java
│   │   │   │           │   │   ├── ☕ ShiftReportServiceImpl.java
│   │   │   │           │   │   ├── ☕ StoreAnalyticsServiceImpl.java
│   │   │   │           │   │   ├── ☕ StoreServiceImpl.java
│   │   │   │           │   │   ├── ☕ SubscriptionPlanServiceImpl.java
│   │   │   │           │   │   ├── ☕ SubscriptionServiceImpl.java
│   │   │   │           │   │   └── ☕ UserServiceImpl.java
│   │   │   │           │   ├── ☕ AdminDashboardService.java
│   │   │   │           │   ├── ☕ AuthService.java
│   │   │   │           │   ├── ☕ BranchAnalyticsService.java
│   │   │   │           │   ├── ☕ BranchService.java
│   │   │   │           │   ├── ☕ CategoryService.java
│   │   │   │           │   ├── ☕ CustomerService.java
│   │   │   │           │   ├── ☕ EmailService.java
│   │   │   │           │   ├── ☕ EmployeeService.java
│   │   │   │           │   ├── ☕ InventoryService.java
│   │   │   │           │   ├── ☕ OrderService.java
│   │   │   │           │   ├── ☕ PaymentService.java
│   │   │   │           │   ├── ☕ ProductService.java
│   │   │   │           │   ├── ☕ RefundService.java
│   │   │   │           │   ├── ☕ ShiftReportService.java
│   │   │   │           │   ├── ☕ StoreAnalyticsService.java
│   │   │   │           │   ├── ☕ StoreService.java
│   │   │   │           │   ├── ☕ SubscriptionPlanService.java
│   │   │   │           │   ├── ☕ SubscriptionService.java
│   │   │   │           │   └── ☕ UserService.java
│   │   │   │           ├── 📁 util
│   │   │   │           │   └── ☕ SecurityUtil.java
│   │   │   │           └── ☕ PosSystemApplication.java
│   │   │   └── 📁 resources
│   │   │       ├── 📁 static
│   │   │       ├── 📁 templates
│   │   │       ├── ⚙️ application.yml
│   │   │       └── ⚙️ docker-compose.yml
│   │   └── 📁 test
│   │       └── 📁 java
│   │           └── 📁 com
│   │               └── 📁 zosh
│   │                   └── ☕ PosSystemApplicationTests.java
│   ├── ⚙️ .gitattributes
│   ├── ⚙️ .gitignore
│   ├── 📝 HELP.md
│   ├── 📄 mvnw
│   ├── 📄 mvnw.cmd
│   └── ⚙️ pom.xml
├── 📁 pos-frontend-vite
│   ├── 📁 public
│   │   ├── 🖼️ benefits-illustration.svg
│   │   ├── 🖼️ branch-management-preview.svg
│   │   ├── 🖼️ header-preview.svg
│   │   ├── 🖼️ landing-page-preview.svg
│   │   ├── 🖼️ pos-mockup.svg
│   │   ├── 🖼️ trusted-logos-preview.svg
│   │   └── 🖼️ vite.svg
│   ├── 📁 src
│   │   ├── 📁 Redux Toolkit
│   │   │   ├── 📁 features
│   │   │   │   ├── 📁 adminDashboard
│   │   │   │   │   ├── 📄 adminDashboardSlice.js
│   │   │   │   │   └── 📄 adminDashboardThunks.js
│   │   │   │   ├── 📁 auth
│   │   │   │   │   ├── 📄 authSlice.js
│   │   │   │   │   └── 📄 authThunk.js
│   │   │   │   ├── 📁 branch
│   │   │   │   │   ├── 📄 branchSlice.js
│   │   │   │   │   └── 📄 branchThunks.js
│   │   │   │   ├── 📁 branchAnalytics
│   │   │   │   │   ├── 📄 branchAnalyticsSlice.js
│   │   │   │   │   └── 📄 branchAnalyticsThunks.js
│   │   │   │   ├── 📁 cart
│   │   │   │   │   └── 📄 cartSlice.js
│   │   │   │   ├── 📁 category
│   │   │   │   │   ├── 📄 categorySlice.js
│   │   │   │   │   └── 📄 categoryThunks.js
│   │   │   │   ├── 📁 customer
│   │   │   │   │   ├── 📄 customerSlice.js
│   │   │   │   │   └── 📄 customerThunks.js
│   │   │   │   ├── 📁 employee
│   │   │   │   │   ├── 📄 employeeSlice.js
│   │   │   │   │   └── 📄 employeeThunks.js
│   │   │   │   ├── 📁 inventory
│   │   │   │   │   ├── 📄 inventorySlice.js
│   │   │   │   │   └── 📄 inventoryThunks.js
│   │   │   │   ├── 📁 onboarding
│   │   │   │   │   ├── 📄 onboardingSlice.js
│   │   │   │   │   └── 📄 onboardingThunk.js
│   │   │   │   ├── 📁 order
│   │   │   │   │   ├── 📄 orderSlice.js
│   │   │   │   │   └── 📄 orderThunks.js
│   │   │   │   ├── 📁 payment
│   │   │   │   │   ├── 📄 paymentSlice.js
│   │   │   │   │   └── 📄 paymentThunks.js
│   │   │   │   ├── 📁 product
│   │   │   │   │   ├── 📄 productSlice.js
│   │   │   │   │   └── 📄 productThunks.js
│   │   │   │   ├── 📁 refund
│   │   │   │   │   ├── 📄 refundSlice.js
│   │   │   │   │   └── 📄 refundThunks.js
│   │   │   │   ├── 📁 sale
│   │   │   │   │   ├── 📄 saleSlice.js
│   │   │   │   │   └── 📄 saleThunks.js
│   │   │   │   ├── 📁 shiftReport
│   │   │   │   │   ├── 📄 shiftReportSlice.js
│   │   │   │   │   └── 📄 shiftReportThunks.js
│   │   │   │   ├── 📁 store
│   │   │   │   │   ├── 📄 storeSlice.js
│   │   │   │   │   └── 📄 storeThunks.js
│   │   │   │   ├── 📁 storeAnalytics
│   │   │   │   │   ├── 📄 storeAnalyticsSlice.js
│   │   │   │   │   └── 📄 storeAnalyticsThunks.js
│   │   │   │   ├── 📁 subscription
│   │   │   │   │   ├── 📄 subscriptionSlice.js
│   │   │   │   │   └── 📄 subscriptionThunks.js
│   │   │   │   ├── 📁 subscriptionPlan
│   │   │   │   │   ├── 📄 subscriptionPlanSlice.js
│   │   │   │   │   └── 📄 subscriptionPlanThunks.js
│   │   │   │   ├── 📁 transaction
│   │   │   │   │   ├── 📄 transactionSlice.js
│   │   │   │   │   └── 📄 transactionThunks.js
│   │   │   │   └── 📁 user
│   │   │   │       ├── 📄 userSlice.js
│   │   │   │       └── 📄 userThunks.js
│   │   │   └── 📄 globleState.js
│   │   ├── 📁 assets
│   │   │   └── 🖼️ react.svg
│   │   ├── 📁 components
│   │   │   ├── 📁 ui
│   │   │   │   ├── 📄 accordion.jsx
│   │   │   │   ├── 📄 alert-dialog.jsx
│   │   │   │   ├── 📄 alert.jsx
│   │   │   │   ├── 📄 aspect-ratio.jsx
│   │   │   │   ├── 📄 avatar.jsx
│   │   │   │   ├── 📄 badge.jsx
│   │   │   │   ├── 📄 breadcrumb.jsx
│   │   │   │   ├── 📄 button.jsx
│   │   │   │   ├── 📄 calendar.jsx
│   │   │   │   ├── 📄 card.jsx
│   │   │   │   ├── 📄 carousel.jsx
│   │   │   │   ├── 📄 chart.jsx
│   │   │   │   ├── 📄 checkbox.jsx
│   │   │   │   ├── 📄 collapsible.jsx
│   │   │   │   ├── 📄 command.jsx
│   │   │   │   ├── 📄 context-menu.jsx
│   │   │   │   ├── 📄 dialog.jsx
│   │   │   │   ├── 📄 drawer.jsx
│   │   │   │   ├── 📄 dropdown-menu.jsx
│   │   │   │   ├── 📄 form.jsx
│   │   │   │   ├── 📄 hover-card.jsx
│   │   │   │   ├── 📄 input-otp.jsx
│   │   │   │   ├── 📄 input.jsx
│   │   │   │   ├── 📄 label.jsx
│   │   │   │   ├── 📄 menubar.jsx
│   │   │   │   ├── 📄 navigation-menu.jsx
│   │   │   │   ├── 📄 pagination.jsx
│   │   │   │   ├── 📄 popover.jsx
│   │   │   │   ├── 📄 progress.jsx
│   │   │   │   ├── 📄 radio-group.jsx
│   │   │   │   ├── 📄 resizable.jsx
│   │   │   │   ├── 📄 scroll-area.jsx
│   │   │   │   ├── 📄 select.jsx
│   │   │   │   ├── 📄 separator.jsx
│   │   │   │   ├── 📄 sheet.jsx
│   │   │   │   ├── 📄 sidebar.jsx
│   │   │   │   ├── 📄 skeleton.jsx
│   │   │   │   ├── 📄 slider.jsx
│   │   │   │   ├── 📄 sonner.jsx
│   │   │   │   ├── 📄 switch.jsx
│   │   │   │   ├── 📄 table.jsx
│   │   │   │   ├── 📄 tabs.jsx
│   │   │   │   ├── 📄 textarea.jsx
│   │   │   │   ├── 📄 toast.jsx
│   │   │   │   ├── 📄 toggle-group.jsx
│   │   │   │   ├── 📄 toggle.jsx
│   │   │   │   ├── 📄 tooltip.jsx
│   │   │   │   └── 📄 use-toast.jsx
│   │   │   ├── 📄 theme-provider.jsx
│   │   │   └── 📄 theme-toggle.jsx
│   │   ├── 📁 context
│   │   │   ├── 📁 hooks
│   │   │   │   └── 📄 useSidebar.js
│   │   │   ├── 📄 SidebarContext.jsx
│   │   │   └── 📄 SidebarProvider.jsx
│   │   ├── 📁 contexts
│   │   ├── 📁 hooks
│   │   │   └── 📄 use-mobile.js
│   │   ├── 📁 lib
│   │   │   └── 📄 utils.js
│   │   ├── 📁 pages
│   │   │   ├── 📁 Branch Manager
│   │   │   │   ├── 📁 Customers
│   │   │   │   │   └── 📄 Customers.jsx
│   │   │   │   ├── 📁 Dashboard
│   │   │   │   │   ├── 📄 BranchManagerDashboard.jsx
│   │   │   │   │   ├── 📄 BranchManagerSidebar.jsx
│   │   │   │   │   ├── 📄 BranchManagerTopbar.jsx
│   │   │   │   │   ├── 📄 CashierPerformance.jsx
│   │   │   │   │   ├── 📄 Dashboard.jsx
│   │   │   │   │   ├── 📄 PaymentBreakdown.jsx
│   │   │   │   │   ├── 📄 RecentOrders.jsx
│   │   │   │   │   ├── 📄 SalesChart.jsx
│   │   │   │   │   ├── 📄 TodayOverview.jsx
│   │   │   │   │   └── 📄 TopProducts.jsx
│   │   │   │   ├── 📁 Employees
│   │   │   │   │   ├── 📄 BranchEmployees.jsx
│   │   │   │   │   ├── 📄 EmployeeDialogs.jsx
│   │   │   │   │   ├── 📄 EmployeeStats.jsx
│   │   │   │   │   ├── 📄 EmployeeTable.jsx
│   │   │   │   │   └── 📄 index.js
│   │   │   │   ├── 📁 Inventory
│   │   │   │   │   ├── 📄 Inventory.jsx
│   │   │   │   │   ├── 📄 InventoryFilters.jsx
│   │   │   │   │   ├── 📄 InventoryFormDialog.jsx
│   │   │   │   │   ├── 📄 InventoryStats.jsx
│   │   │   │   │   ├── 📄 InventoryTable.jsx
│   │   │   │   │   └── 📄 ProductSelect.jsx
│   │   │   │   ├── 📁 Orders
│   │   │   │   │   ├── 📄 OrderDetailsDialog.jsx
│   │   │   │   │   ├── 📄 Orders.jsx
│   │   │   │   │   ├── 📄 OrdersFilters.jsx
│   │   │   │   │   ├── 📄 OrdersTable.jsx
│   │   │   │   │   └── 📄 data.js
│   │   │   │   ├── 📁 Refunds
│   │   │   │   │   └── 📄 Refunds.jsx
│   │   │   │   ├── 📁 Reports
│   │   │   │   │   └── 📄 Reports.jsx
│   │   │   │   ├── 📁 Settings
│   │   │   │   │   ├── 📄 BranchInfo.jsx
│   │   │   │   │   └── 📄 Settings.jsx
│   │   │   │   ├── 📁 Transaction
│   │   │   │   │   ├── 📄 TransactionTable.jsx
│   │   │   │   │   └── 📄 Transactions.jsx
│   │   │   │   ├── 📄 data.js
│   │   │   │   └── 📄 index.js
│   │   │   ├── 📁 SuperAdminDashboard
│   │   │   │   ├── 📁 components
│   │   │   │   │   ├── 📄 SuperAdminSidebar.jsx
│   │   │   │   │   ├── 📄 SuperAdminTopbar.jsx
│   │   │   │   │   └── 📄 index.js
│   │   │   │   ├── 📁 settings
│   │   │   │   │   ├── 📁 components
│   │   │   │   │   │   ├── 📄 NotificationSettingsForm.jsx
│   │   │   │   │   │   ├── 📄 ProfileSettingsForm.jsx
│   │   │   │   │   │   ├── 📄 SecuritySettingsForm.jsx
│   │   │   │   │   │   ├── 📄 SystemSettingsForm.jsx
│   │   │   │   │   │   └── 📄 useSettingsState.js
│   │   │   │   │   └── 📄 SettingsPage.jsx
│   │   │   │   ├── 📁 store
│   │   │   │   │   ├── 📄 PendingRequestsPage.jsx
│   │   │   │   │   ├── 📄 StoreDetailDrawer.jsx
│   │   │   │   │   ├── 📄 StoreDetailsPage.jsx
│   │   │   │   │   ├── 📄 StoreListPage.jsx
│   │   │   │   │   ├── 📄 StoreStatusBadge.jsx
│   │   │   │   │   └── 📄 StoreTable.jsx
│   │   │   │   ├── 📁 subscription
│   │   │   │   │   ├── 📄 AddPlanDialog.jsx
│   │   │   │   │   ├── 📄 EditPlanDialog.jsx
│   │   │   │   │   └── 📄 SubscriptionPlansPage.jsx
│   │   │   │   ├── 📄 CommissionsPage.jsx
│   │   │   │   ├── 📄 Dashboard.jsx
│   │   │   │   ├── 📄 ExportsPage.jsx
│   │   │   │   ├── 📝 README.md
│   │   │   │   ├── 📄 SuperAdminDashboard.jsx
│   │   │   │   └── 📄 index.js
│   │   │   ├── 📁 auth
│   │   │   ├── 📁 cashier
│   │   │   │   ├── 📁 ShiftSummary
│   │   │   │   │   ├── 📁 components
│   │   │   │   │   │   ├── 📄 LogoutConfirmDialog.jsx
│   │   │   │   │   │   ├── 📄 PaymentSummaryCard.jsx
│   │   │   │   │   │   ├── 📄 PrintDialog.jsx
│   │   │   │   │   │   ├── 📄 RecentOrdersCard.jsx
│   │   │   │   │   │   ├── 📄 RefundsCard.jsx
│   │   │   │   │   │   ├── 📄 SalesSummaryCard.jsx
│   │   │   │   │   │   ├── 📄 ShiftHeader.jsx
│   │   │   │   │   │   ├── 📄 ShiftInformationCard.jsx
│   │   │   │   │   │   ├── 📄 TopSellingItemsCard.jsx
│   │   │   │   │   │   └── 📄 index.js
│   │   │   │   │   ├── 📁 data
│   │   │   │   │   │   └── 📄 mockShiftData.js
│   │   │   │   │   └── 📄 ShiftSummaryPage.jsx
│   │   │   │   ├── 📁 Sidebar
│   │   │   │   │   ├── 📄 BranchInfo.jsx
│   │   │   │   │   ├── 📄 CashierSideBar.jsx
│   │   │   │   │   └── 📄 navItems.js
│   │   │   │   ├── 📁 cart
│   │   │   │   │   ├── 📄 CartItem.jsx
│   │   │   │   │   ├── 📄 CartSection.jsx
│   │   │   │   │   └── 📄 CartSummary.jsx
│   │   │   │   ├── 📁 components
│   │   │   │   │   ├── 📄 HeldOrdersDialog.jsx
│   │   │   │   │   ├── 📄 POSHeader.jsx
│   │   │   │   │   └── 📄 ReceiptDialog.jsx
│   │   │   │   ├── 📁 customer
│   │   │   │   │   ├── 📁 components
│   │   │   │   │   │   ├── 📄 AddPointsDialog.jsx
│   │   │   │   │   │   ├── 📄 CustomerCard.jsx
│   │   │   │   │   │   ├── 📄 CustomerDetails.jsx
│   │   │   │   │   │   ├── 📄 CustomerList.jsx
│   │   │   │   │   │   ├── 📄 CustomerSearch.jsx
│   │   │   │   │   │   ├── 📄 PurchaseHistory.jsx
│   │   │   │   │   │   └── 📄 index.js
│   │   │   │   │   ├── 📁 data
│   │   │   │   │   ├── 📁 utils
│   │   │   │   │   │   └── 📄 customerUtils.js
│   │   │   │   │   ├── 📄 CustomerDialog.jsx
│   │   │   │   │   ├── 📄 CustomerForm.jsx
│   │   │   │   │   └── 📄 CustomerLookupPage.jsx
│   │   │   │   ├── 📁 order
│   │   │   │   │   ├── 📁 OrderDetails
│   │   │   │   │   │   ├── 📄 CustomerInformation.jsx
│   │   │   │   │   │   ├── 📄 InvoiceDialog.jsx
│   │   │   │   │   │   ├── 📄 OrderDetails.jsx
│   │   │   │   │   │   └── 📄 OrderInformation.jsx
│   │   │   │   │   ├── 📁 pdf
│   │   │   │   │   │   ├── 📄 OrderPDF.jsx
│   │   │   │   │   │   ├── 📄 pdfStyles.jsx
│   │   │   │   │   │   └── 📄 pdfUtils.jsx
│   │   │   │   │   ├── 📄 OrderHistoryPage.jsx
│   │   │   │   │   ├── 📄 OrderTable.jsx
│   │   │   │   │   └── 📄 data.js
│   │   │   │   ├── 📁 payment
│   │   │   │   │   ├── 📄 CustomerPaymentSection.jsx
│   │   │   │   │   ├── 📄 CustomerSection.jsx
│   │   │   │   │   ├── 📄 DiscountSection.jsx
│   │   │   │   │   ├── 📄 NoteSection.jsx
│   │   │   │   │   ├── 📄 PaymentDialog.jsx
│   │   │   │   │   ├── 📄 PaymentSection.jsx
│   │   │   │   │   └── 📄 data.js
│   │   │   │   ├── 📁 product
│   │   │   │   │   ├── 📄 ProductCard.jsx
│   │   │   │   │   └── 📄 ProductSection.jsx
│   │   │   │   ├── 📁 return
│   │   │   │   │   ├── 📁 components
│   │   │   │   │   │   ├── 📄 OrderDetailsSection.jsx
│   │   │   │   │   │   ├── 📄 OrderTable.jsx
│   │   │   │   │   │   ├── 📄 ReturnItemsSection.jsx
│   │   │   │   │   │   ├── 📄 ReturnReceiptDialog.jsx
│   │   │   │   │   │   └── 📄 index.js
│   │   │   │   │   └── 📄 ReturnOrderPage.jsx
│   │   │   │   ├── 📄 CashierDashboardLayout.jsx
│   │   │   │   ├── 📄 CreateOrderPage.jsx
│   │   │   │   └── 📝 README.md
│   │   │   ├── 📁 common
│   │   │   │   ├── 📁 Auth
│   │   │   │   │   ├── 📄 Login.jsx
│   │   │   │   │   └── 📄 ResetPassword.jsx
│   │   │   │   ├── 📁 Demo
│   │   │   │   ├── 📁 Landing
│   │   │   │   │   ├── 📁 components
│   │   │   │   │   │   ├── 📄 TypewriterText.jsx
│   │   │   │   │   │   └── 📄 index.js
│   │   │   │   │   ├── 📄 ContactSection.jsx
│   │   │   │   │   ├── 📄 FAQSection.jsx
│   │   │   │   │   ├── 📄 FeatureComparisonSection.jsx
│   │   │   │   │   ├── 📄 FeatureComparisonTable.jsx
│   │   │   │   │   ├── 📄 FetureSection.jsx
│   │   │   │   │   ├── 📄 Footer.jsx
│   │   │   │   │   ├── 📄 Header.jsx
│   │   │   │   │   ├── 📄 HeroSection.jsx
│   │   │   │   │   ├── 📄 KeyFeaturesSection.jsx
│   │   │   │   │   ├── 📄 Landing.jsx
│   │   │   │   │   ├── 📄 LiveDemoSection.jsx
│   │   │   │   │   ├── 📄 MobileAppShowcase.jsx
│   │   │   │   │   ├── 📄 PricingCalculator.jsx
│   │   │   │   │   ├── 📄 PricingSection.jsx
│   │   │   │   │   ├── 📄 TestimonialCarousel.jsx
│   │   │   │   │   ├── 📄 TrustedLogos.jsx
│   │   │   │   │   └── 📄 WhyChooseUsSection.jsx
│   │   │   │   ├── 📁 Order
│   │   │   │   │   └── 📄 OrderItemTable.jsx
│   │   │   │   └── 📄 PageNotFound.jsx
│   │   │   ├── 📁 components
│   │   │   ├── 📁 onboarding
│   │   │   │   ├── 📄 Onboarding.jsx
│   │   │   │   ├── 📄 OwnerDetailsForm.jsx
│   │   │   │   ├── 📝 README.md
│   │   │   │   ├── 📄 StoreDetailsForm.jsx
│   │   │   │   └── 📄 index.js
│   │   │   └── 📁 store
│   │   │       ├── 📁 Alerts
│   │   │       │   ├── 📄 Alerts.jsx
│   │   │       │   ├── 📄 InactiveCashierTable.jsx
│   │   │       │   ├── 📄 LowStockProductTable.jsx
│   │   │       │   ├── 📄 NoSaleTodayBranchTable.jsx
│   │   │       │   └── 📄 RefundSpikeTable.jsx
│   │   │       ├── 📁 Branch
│   │   │       │   ├── 📄 BranchForm.jsx
│   │   │       │   ├── 📄 BranchTable.jsx
│   │   │       │   ├── 📄 Branches.jsx
│   │   │       │   └── 📄 index.js
│   │   │       ├── 📁 Category
│   │   │       │   ├── 📄 Categories.jsx
│   │   │       │   ├── 📄 CategoryForm.jsx
│   │   │       │   ├── 📄 CategoryTable.jsx
│   │   │       │   └── 📄 index.js
│   │   │       ├── 📁 Dashboard
│   │   │       │   ├── 📄 Dashboard.jsx
│   │   │       │   ├── 📄 DashboardStats.jsx
│   │   │       │   ├── 📄 RecentSales.jsx
│   │   │       │   ├── 📄 SalesTrend.jsx
│   │   │       │   ├── 📄 StoreDashboard.jsx
│   │   │       │   ├── 📄 StoreSidebar.jsx
│   │   │       │   ├── 📄 StoreTopbar.jsx
│   │   │       │   └── 📄 index.js
│   │   │       ├── 📁 Employee
│   │   │       │   ├── 📄 EmployeeForm.jsx
│   │   │       │   ├── 📄 EmployeeTable.jsx
│   │   │       │   ├── 📄 StoreEmployees.jsx
│   │   │       │   └── 📄 index.js
│   │   │       ├── 📁 Product
│   │   │       │   ├── 📄 CreateProductForm.jsx
│   │   │       │   ├── 📄 ProductDetails.jsx
│   │   │       │   ├── 📄 ProductForm.jsx
│   │   │       │   ├── 📄 ProductSearch.jsx
│   │   │       │   ├── 📄 ProductTable.jsx
│   │   │       │   ├── 📄 Products.jsx
│   │   │       │   └── 📄 index.js
│   │   │       ├── 📁 Settings
│   │   │       │   ├── 📁 components
│   │   │       │   │   ├── 📄 NotificationSettings.jsx
│   │   │       │   │   ├── 📄 PaymentSettings.jsx
│   │   │       │   │   ├── 📄 SecuritySettings.jsx
│   │   │       │   │   ├── 📄 SettingsContent.jsx
│   │   │       │   │   ├── 📄 SettingsHeader.jsx
│   │   │       │   │   ├── 📄 SettingsNavigation.jsx
│   │   │       │   │   ├── 📄 StoreSettings.jsx
│   │   │       │   │   ├── 📄 StoreSettingsForm.jsx
│   │   │       │   │   ├── 📄 ToggleSwitch.jsx
│   │   │       │   │   ├── 📄 formUtils.js
│   │   │       │   │   ├── 📄 index.js
│   │   │       │   │   └── 📄 validation.js
│   │   │       │   └── 📄 Settings.jsx
│   │   │       ├── 📁 store-admin
│   │   │       │   ├── 📄 Reports.jsx
│   │   │       │   ├── 📄 Sales.jsx
│   │   │       │   └── 📄 index.js
│   │   │       ├── 📁 storeInformation
│   │   │       │   ├── 📁 components
│   │   │       │   │   ├── 📄 BasicInformation.jsx
│   │   │       │   │   ├── 📄 ContactInformation.jsx
│   │   │       │   │   ├── 📄 EditStoreDialog.jsx
│   │   │       │   │   ├── 📄 EditStoreForm.jsx
│   │   │       │   │   ├── 📄 EmptyState.jsx
│   │   │       │   │   ├── 📄 LoadingState.jsx
│   │   │       │   │   ├── 📄 StoreHeader.jsx
│   │   │       │   │   ├── 📄 StoreInfoCard.jsx
│   │   │       │   │   ├── 📄 formUtils.js
│   │   │       │   │   ├── 📄 index.js
│   │   │       │   │   └── 📄 validation.js
│   │   │       │   └── 📄 Stores.jsx
│   │   │       └── 📁 upgrade
│   │   │           └── 📄 Upgrade.jsx
│   │   ├── 📁 routes
│   │   │   ├── 📄 AuthRoutes.jsx
│   │   │   ├── 📄 BranchManagerRoutes.jsx
│   │   │   ├── 📄 CashierRoutes.jsx
│   │   │   ├── 📄 StoreRoutes.jsx
│   │   │   └── 📄 SuperAdminRoutes.jsx
│   │   ├── 📁 utils
│   │   │   ├── 📄 api.js
│   │   │   ├── 📄 formateDate.js
│   │   │   ├── 📄 getPaymentIcon.jsx
│   │   │   ├── 📄 getStatusColor.js
│   │   │   ├── 📄 paymentMethodLable.js
│   │   │   ├── 📄 uploadToCloudinary.js
│   │   │   └── 📄 userRole.js
│   │   ├── 🎨 App.css
│   │   ├── 📄 App.jsx
│   │   ├── 🎨 index.css
│   │   └── 📄 main.jsx
│   ├── ⚙️ .gitignore
│   ├── 📝 README.md
│   ├── ⚙️ components.json
│   ├── 📄 eslint.config.js
│   ├── 🌐 index.html
│   ├── ⚙️ jsconfig.app.json
│   ├── ⚙️ jsconfig.json
│   ├── ⚙️ package.json
│   ├── ⚙️ pnpm-lock.yaml
│   └── 📄 vite.config.js
└── 📝 README.md
```

---

_Generated by FileTree Pro Extension_

## 📡 API Overview

| Method | Endpoint             | Description           |
| ------ | -------------------- | --------------------- |
| `POST` | `/api/auth/login`    | User login            |
| `POST` | `/api/auth/register` | Register a new user   |
| `GET`  | `/api/products`      | Retrieve product list |
| `POST` | `/api/orders`        | Create a new order    |
| `GET`  | `/api/reports/sales` | Get sales report      |

> Full API documentation is available in Swagger at:
> UPDATING SOON...

---

## 🧪 Testing

- Unit Testing with **JUnit & Mockito**
- Integration Testing with database
- Manual testing of key workflows (POS billing, admin panel, reports)

---

## 🖼️ Screenshots (COMING SOON)

_(Include screenshots here)_

- POS Terminal Interface
- Inventory Management Page
- Dashboard Analytics
- Admin Control Panel

---

## 🔮 Future Enhancements

- 📱 Mobile App Support (React Native / Flutter)
- 🧾 Barcode & QR Code Scanning
- 🤖 AI-based Sales Predictions
- 📴 Offline Mode Support

---

## 👨‍💻 Contributors

| Name                    | Role                 |
| ----------------------- | -------------------- |
| **Satinder Singh Sall** | Full Stack Developer |

---

## 📜 License

This project is licensed under the **MIT License** – feel free to use and modify for educational or commercial purposes.

---

> 💡 _“Empowering Retail Through Automation.”_

```

```
