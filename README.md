# Rydex -- Car Booking Platform

Rydex is a full-stack ride booking platform which allows passengers to book rides, drivers to accept
rides, and admins to manage the platform.
# Project Overview

The platform includes three main roles.

## Passenger

-   Book rides
-   View ride history
-   Make payments
-   Rate drivers
-   Apply promo codes

## Driver

-   Register as a driver
-   Accept or reject ride requests
-   View trip details
-   Manage ride status

## Admin

-   Manage users and drivers
-   Monitor rides
-   Manage promo codes
-   Handle support tickets


# Technologies Used

## Frontend

-   React
-   TypeScript
-   Vite

## Backend

-   Java Spring Boot
-   Spring Security
-   JWT Authentication
-   WebSockets for real-time updates
-   Redis
-   Maven

## Payments

-   Stripe Payment Gateway

## Database

-   JPA / Hibernate

# Main Features

## User Features

-   Register and login
-   Book rides
-   View ride history
-   Make payments
-   Rate drivers
-   Apply promo codes

## Driver Features

-   Driver dashboard
-   Accept ride requests
-   Manage rides
-   View trip history

## Admin Features

-   Admin dashboard
-   Manage users and drivers
-   Monitor rides
-   Manage promo codes
-   Handle support tickets


# Project Structure

    rydex-booking-app/
    │
    ├── frontend/
    │   │
    │   ├── index.html
    │   ├── package.json
    │   ├── vite.config.ts
    │   │
    │   └── src/
    │       │
    │       ├── main.tsx
    │       ├── App.tsx
    │       │
    │       ├── components/
    │       │   ├── MapView.tsx
    │       │   ├── SideDrawer.tsx
    │       │   ├── BookingPanel.tsx
    │       │   ├── LocationCard.tsx
    │       │   │
    │       │   └── Views/
    │       │       ├── HistoryView.tsx
    │       │       ├── PaymentsView.tsx
    │       │       ├── RewardsView.tsx
    │       │       ├── SettingsView.tsx
    │       │       ├── HelpView.tsx
    │       │       ├── SafetyView.tsx
    │       │       ├── AboutView.tsx
    │       │       ├── DriverDashboardView.tsx
    │       │       └── AdminDashboardView.tsx
    │       │
    │       ├── context/
    │       │   └── AppContext.tsx
    │       │
    │       ├── types/
    │       │   └── index.ts
    │       │
    │       └── utils/
    │           └── cn.ts
    │
    ├── backend/
    │   │
    │   ├── pom.xml
    │   │
    │   └── src/main/java/com/rydex
    │       │
    │       ├── RydexApplication.java
    │       │
    │       ├── config/
    │       │   ├── SecurityConfig.java
    │       │   ├── WebSocketConfig.java
    │       │   ├── RedisConfig.java
    │       │   ├── JpaConfig.java
    │       │   └── StripeConfig.java
    │       │
    │       ├── controller/
    │       │   ├── AuthController.java
    │       │   ├── RideController.java
    │       │   ├── DriverController.java
    │       │   ├── PaymentController.java
    │       │   ├── RatingController.java
    │       │   ├── AdminController.java
    │       │   └── WebSocketController.java
    │       │
    │       ├── service/
    │       │   ├── AuthService.java
    │       │   ├── RideService.java
    │       │   ├── DriverService.java
    │       │   ├── PaymentService.java
    │       │   ├── RatingService.java
    │       │   ├── AdminService.java
    │       │   ├── FareCalculationService.java
    │       │   ├── PromoCodeService.java
    │       │   └── EmailService.java
    │       │
    │       ├── repository/
    │       │   ├── UserRepository.java
    │       │   ├── DriverRepository.java
    │       │   ├── RideRepository.java
    │       │   ├── PaymentRepository.java
    │       │   ├── RatingRepository.java
    │       │   ├── PromoCodeRepository.java
    │       │   └── SupportTicketRepository.java
    │       │
    │       ├── entity/
    │       │   ├── User.java
    │       │   ├── Driver.java
    │       │   ├── Ride.java
    │       │   ├── Payment.java
    │       │   ├── Rating.java
    │       │   ├── PromoCode.java
    │       │   └── SupportTicket.java
    │       │
    │       ├── dto/
    │       │   ├── auth/
    │       │   │   ├── RegisterRequest.java
    │       │   │   ├── LoginRequest.java
    │       │   │   ├── DriverRegisterRequest.java
    │       │   │   └── AuthResponse.java
    │       │   │
    │       │   ├── ride/
    │       │   │   ├── RideRequestDto.java
    │       │   │   ├── RideResponseDto.java
    │       │   │   └── FareEstimateDto.java
    │       │   │
    │       │   ├── payment/
    │       │   │   ├── PaymentRequestDto.java
    │       │   │   └── PaymentResponseDto.java
    │       │   │
    │       │   └── rating/
    │       │       ├── RatingRequestDto.java
    │       │       └── RatingResponseDto.java
    │       │
    │       ├── security/
    │       │   ├── JwtTokenProvider.java
    │       │   ├── JwtAuthenticationFilter.java
    │       │   ├── CustomUserDetails.java
    │       │   ├── CustomUserDetailsService.java
    │       │   └── OAuth2AuthenticationSuccessHandler.java
    │       │
    │       └── exception/
    │           ├── BadRequestException.java
    │           ├── ResourceNotFoundException.java
    │           └── GlobalExceptionHandler.java
    │
    └── README.md


# Setup Instructions

## 1. Clone the Repository

git clone "paste the repo link here"


## 2. Run Backend

Navigate to the backend folder and run:

mvn spring-boot:run

## 3. Run Frontend

Navigate to the frontend folder and run:

npm install

npm run dev


# Environment Configuration

You will need to configure:

-   Database connection
-   Stripe API keys
-   JWT secret key
-   Redis configuration

These settings are usually placed inside:

application.properties\
\
application.yml

# Future Improvements

Possible improvements for the platform:

-   Mobile application
-   Live driver tracking
-   Push notification system
