[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/IIp1tMqN)
---
title: Experiment 3 - Ticket Booking System with Synchronized Threads
---

# Experiment 3 - Ticket Booking System with Synchronized Threads

## Objective
To develop a ticket booking system using synchronized threads to prevent double booking of seats. The system will also utilize thread priorities to simulate VIP bookings being processed first.

## Description
In this experiment, we implement a multi-threaded ticket booking system where:
- Multiple users (threads) attempt to book seats simultaneously.
- Synchronization is used to prevent double booking of the same seat.
- Thread priorities are set to give VIP bookings higher precedence over regular bookings.

## Features
- **Synchronized Booking**: Ensures that no two threads book the same seat at the same time.
- **Thread Priorities**: VIP bookings are handled first by assigning them higher priority.
- **Concurrency Handling**: Manages multiple users booking tickets concurrently without conflicts.

## Implementation Steps
1. **Create a `TicketBookingSystem` class** that maintains available seats.
2. **Implement synchronization** in the booking method to prevent seat overbooking.
3. **Create `VIPUser` and `RegularUser` classes** extending `Thread`.
4. **Assign thread priorities** (higher for VIP users) to process their bookings first.
5. **Simulate multiple users booking tickets** simultaneously.
6. **Print booking status** to verify synchronization and priority handling.

## Sample Output
```
VIP User 1 booked Seat 5
VIP User 2 booked Seat 6
Regular User 1 booked Seat 7
Regular User 2 booked Seat 8
```
This ensures that VIP users' bookings are processed first while maintaining synchronization.

## Complexity Analysis
- **Synchronization Overhead**: O(n), where `n` is the number of booking attempts.
- **Thread Execution Order**: VIP users are prioritized, but execution depends on the thread scheduler.

## Conclusion
This experiment demonstrates how to use Java threads, synchronization, and priority settings to implement a reliable ticket booking system. The use of thread synchronization prevents double booking, while thread priority ensures that VIP bookings are processed first.

## License
This project is open-source and available for educational purposes.

