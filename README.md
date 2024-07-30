# Exam Diagram Repository

Here is the Link for the Diagram that i created from Draw.io
https://drive.google.com/file/d/1Xkmhr9-wEDLBHl54H3CrM3Ult570qUaB/view?usp=sharing

This repository contains a diagram created for an exam.

## Contents

- Diagram files

## Purpose

The purpose of this repository is to store and manage the diagram for the exam.

## Use Cases

-Registration
New users must register and log in before participating in the auction.
Required data: full name, email address, phone number.
User authorization: normal user, administrator.

-Bidding
All registered users can see the details of the auctions.
Users can create a new auction with car brand, year, type, price, bid price increment, and expiry date.
Users can bid on any open auction.
Opening price is set by the admin.
Only the quickest bid is accepted when multiple people bid at the same time.

-Listing
There can only be one owner for each bid lot.
If there is a bidder, the listing will not close until closed by the owner.
The listing will be permanently deleted if expired without bids.

-Admin
Admin can expire a listing with no winner, permanently deleting the listing.
Admin can close any listing with no bidder, which remains open until closed by the owner.
Expired listings are removed from traffic.



## Diagram Explanation:
-Client (Web Browser): Interacts with the entire system through HTTPS, ensuring secure communication.
-Load Balancer: Distributes incoming traffic and applies rate limiting to prevent abuse.
-Web Server: Uses CSP headers for security and forwards requests to the application server.
-Application Server: Handles the main application logic, divided into frontend and backend services.
-Frontend (React.js): Renders the user interface.
-Backend API (Node.js + Express.js): Handles business logic and data processing.
-Authentication Service (OAuth 2.0 + JWT): Manages user authentication and authorization.
-Database (PostgreSQL): Stores persistent data with optimistic concurrency control for handling bid conflicts.
-Caching Layer (Redis): Provides fast access to frequently accessed data and temporary storage for bid conflicts.
-Message Queue (RabbitMQ): Ensures ordered processing of bids and other time-sensitive operations.
-Static Content (CDN): Delivers static content (e.g., images, stylesheets) efficiently.
-RBAC System: Manages roles and permissions for users, integrated with the backend API.

