# Healthcare Application

![React](https://img.shields.io/badge/ReactJS-v18.0.0-blue.svg)
![NextJS](https://img.shields.io/badge/NextJS-v14.2.4-lightblue.svg)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-v3.4.1-black.svg)

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)

## Project Overview

**Healthcare Application** is built using React JS with Next JS and TypeScript, styled with Tailwind CSS. It features user management where users can sign up, complete their profiles, and schedule multiple appointments. Admin users have a secure OTP-verified dashboard to manage appointments, which includes viewing, rescheduling, and cancelling appointments with statuses such as scheduled, cancelled, and pending. Additionally, users receive SMS notifications when their appointment statuses change. Error tracking is integrated through Sentry to monitor application performance and issues.

## Features

- **Error Tracking:** Integrated with Sentry to track and monitor application errors and performance issues.
- **User Management:**
  - **User Creation:** Users can sign up and complete their profile information.
  - **Appointment Scheduling:** Users can create multiple appointments within the same session.
- **Admin Dashboard:**
  - **OTP Verification:** Admin users can log in securely with One-Time Password (OTP) verification.
  - **Appointment Management:** The dashboard displays all appointments with their statuses (scheduled, cancelled, pending). Admins can reschedule or cancel appointments.
  - **Notifications:** Users receive an SMS notification whenever the status of their appointment changes.

## Technologies Used

- **Frontend**: React.js, Next.js
- **Library**: Appwrite, Sentry, Zod, Twilio
- **Styling**: TailwindCSS

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**:

   ```sh
   git clone https://github.com/SandroSD/patient-management-system.git
   ```

2. **Navigate to the project directory**:

   ```sh
   cd /patient-management-system
   ```

3. **Install frontend dependencies**:

   ```sh
   npm install
   ```

4. **Duplicate .env.sample and rename as .env.local:**

5. **Complete it with the values:**

   ```sh
    PROJECT_ID = #AppWrite Project ID

    API_KEY = #AppWrite API Key

    DATABASE_ID = #AppWrite Database ID

    PATIENT_COLLECTION_ID = #AppWrite Patient Collection ID

    DOCTOR_COLLECTION_ID = #AppWrite Doctor Collection ID

    APPOINTMENT_COLLECTION_ID = #AppWrite Appointment Collection ID

    NEXT_PUBLIC_BUCKET_ID = #AppWrite Bucket (upload images) ID

    NEXT_PUBLIC_ENDPOINT = #AppWrite Endpoint

    NEXT_PUBLIC_ADMIN_PASSKEY = #OTP password for admin dashboard

    SENTRY_AUTH_TOKEN = #Sentry Token for logging actions
   ```

6. **Start the frontend development server**:

   ```sh
   npm run dev
   ```

The application will be available at `http://localhost:3000`.

## Usage

1. Open the application in your browser.

### As Patient

2. Register as a user and complete your medical history information. Then create a new appointment.
3. Once your appointment is created, create as many appointments as you want.

### As Admin

2. Login with the OTP number.
3. You can schedule or cancel any appointment. The patient will receive a SMS notification.
