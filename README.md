# Travel Ra - Firebase Backend

This repository contains backend architecture and database structure used in Travel Ra system.

## Features
- Firebase Authentication
- Realtime Database / Firestore
- Cloud Storage

## Database Structure
1. Authentication
Provider: Firebase Authentication.

Function: Secure login for the Android Mobile Client and encrypted access for the React Admin Panel.

2. Cloud Firestore (NoSQL Database)
The system utilizes a structured collection-document model for real-time data synchronization.

Collections:
users: Stores user profiles (Name, Email, Phone) mapped to unique UIDs.

tour_packages: Dynamic catalog containing titles, descriptions, pricing, and image URLs.

taxi_bookings: Records pickup/drop-off locations, vehicle types, and estimated fares.

vehicles: List of available vehicle categories (Sedan, SUV, Luxury) for the booking engine.

notifications: Real-time alerts and promotional messages triggered by a Firebase listener.

3. Cloud Storage
Purpose: Hosting high-quality media assets.

Optimization: Images are served via the Glide library for efficient caching on mobile devices.

