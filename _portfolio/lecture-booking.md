---
title: Academic Lecture Management and Booking System
layout: project
permalink: /projects/lecture-booking/
order: 1
kind: Java Backend Development
period: Oct 2025–Jun 2026
summary: Developed APIs for managing and booking university lectures, with safeguards against overbooking and duplicate reservations under concurrent requests.
stack: [Java, Spring Boot, MyBatis-Plus, SQL]
---

## Backend APIs

I built the backend with Spring Boot and MyBatis-Plus and independently implemented APIs for **eight core modules** across the admin and user interfaces. These covered access control, lecture publishing, online booking, and reporting.

## Data Modeling and Concurrency

I modeled **eight types of entities**, including users, lectures, reservations, and favorites, and designed the database tables. I used transactions and optimistic locking to prevent overbooking and duplicate reservations when requests arrived concurrently.

![Booking flow showing the request, availability check, and reservation write using a transaction and optimistic locking]({{ '/images/booking-flow.svg' | relative_url }})

## Testing and Performance

I designed functional, performance, and security test cases. SQL query tuning and indexing kept the average response time of core endpoints **under 500 ms in project tests**. I also developed a visualization module for reporting in the admin interface.
