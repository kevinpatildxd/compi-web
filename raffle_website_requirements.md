# Raffle Website Functional Requirements

## 1. Project Overview
**Goal:** Develop a fully functional online Raffle / Competition Platform similar to *The Watch Draws* and *Rusboy Competitions*.
**Core Concept:** A comprehensive platform where users can browse competitions, purchase tickets, participate in draws via skill-based entry, and track their wins. The system includes a robust user portal, an admin dashboard for full site management, and secure payment processing.

---

## 2. User Module
**Objective:** Provide a seamless experience for users to register, manage their profile, and track their participation.

*   **Registration & Login:** Secure email/password login, with optional social login.
*   **Profile Management:** Edit personal details, password, and contact information.
*   **My Wallet:**
    *   View current credit balance.
    *   Deposit funds ("Top-up") for future use.
    *   View transaction history (deposits, spends, cashback).
    *   **Cashback System:** Earn automatic credit back on specific ticket purchases (as seen on Rusboy).
*   **Ticket Management:**
    *   **Active Tickets:** View all tickets for draws that haven't taken place yet.
    *   **Entry History:** Complete archive of past entered competitions.
    *   **Instant Wins:** Immediate notification and logging if a purchased ticket matches a winning number.
*   **Winners Page:** Dedicated section to view past winners and specific "Instant Win" results.

---

## 3. Competition & Ticketing Module
**Objective:** The core engine of the website, handling the display and processing of all raffles.

*   **Competition Display:**
    *   **Hero Slider:** Featured competitions with high-impact visuals.
    *   **Cards:** Grid view showing Prize Name, Ticket Price, and Progress Bar (Sold vs. Total).
    *   **Filters:** Categories for "Live", "Ending Soon", "Sold Out", and "Completed".
*   **Detailed Competition Page:**
    *   **Media:** High-quality image gallery of the prize.
    *   **Live Stats:** Real-time updates on "Tickets Remaining" and "Instant Wins Left".
    *   **Countdown Timer:** Visual urgency indicator for draw deadline.
    *   **Description:** Rich text area for prize details and specs.
*   **Entry Mechanism (Compliance & Flow):**
    *   **Skill-Based Question:** Mandatory question (Math/Trivia) required before adding tickets to cart (Legal Requirement).
    *   **Ticket Selector:** Options for manual quantity input or "Quick Select" buttons (+5, +10).
    *   **Ticket Allocation:**
        *   **Standard:** System assigns next available numbers or randomizes within range.
        *   **Instant Win Logic:** Instant checking of assigned numbers against a pre-set list of winning numbers.
*   **Cart & Checkout:**
    *   Review order summary.
    *   Apply discount/promo codes.
    *   **Wallet Payment:** Option to use available wallet balance partial or full payment.

---

## 4. Admin Module
**Objective:** A powerful backend dashboard for the platform owner to manage the entire business.

*   **Competition Management:**
    *   Create, Edit, Duplicate, and Delete competitions.
    *   Set parameters: Ticket Price, Total Ticket Supply, End Date/Time, Max Tickets Per User.
    *   **Instant Win Setup:** Upload or generate winning ticket numbers and assign prizes to them.
*   **Order & User Management:**
    *   View all customer orders and statuses.
    *   Manage user accounts (reset passwords, manual ban).
    *   **Wallet Adjustments:** Manually credit or debit user wallets (for refunds or bonuses).
*   **Draw Management:**
    *   **Entry Export:** One-click export of Entry List (Name, Ticket #) to CSV for third-party draws.
    *   **Winner Declaration:** input winning number to mark competition as "Completed" and display winner on frontend.
    *   **Winner Gallery:** Upload photos and details to the public "Winners" page.
*   **Content Management:**
    *   Manage static pages (FAQ, Terms & Conditions, Privacy Policy).
    *   Update Homepage banners and promotional text.

---

## 5. Security & Additional Features
*   **Automatic Entry Verification:** System ensures no ticket overselling and verifies valid answers.
*   **Email Alerts:** Automated emails for "Order Confirmation", "Password Reset", "Win Notification", and "Draw Completed".
*   **SEO Structure:** Clean URLs and meta tags for competitions to rank on search engines.
*   **Past Winners Archive:** Permanent searchable record of all previous draws.
