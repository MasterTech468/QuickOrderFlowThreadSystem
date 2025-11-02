# QuickOrderFlowThreadSystem
A multithreaded Java simulation of a fast-paced order processing pipeline — from validation to payment to shipment. Threads coordinate in perfect sequence using wait()/notifyAll(), showcasing thread priority and synchronization in action. Ideal for learning concurrency with a real-world twist!
# QuickOrderFlow

QuickOrderFlow is a Java-based multithreaded simulation of a fast-paced order processing system. It models a real-world flow where orders are validated, payments are processed, and shipments are dispatched — all in a synchronized sequence using thread coordination.

## How It Works

The system uses three threads:
- OrderValidationThread: Initiates and validates the order.
- PaymentThread: Waits for order validation before processing payment.
- ShipmentThread: Waits for payment completion before dispatching shipment.

Thread synchronization is achieved using `wait()` and `notifyAll()` on a shared monitor, ensuring each step executes in the correct order.

##  Features

- Thread priority hints (MAX, NORM, MIN)
- Synchronized execution using `wait()`/`notifyAll()`
- Simple flags to track progress
- Console output for step-by-step visibility

## 🛠 Requirements

- Java 8 or higher
- Any IDE or terminal that supports Java compilation

## 🚦 Run It

bash
javac QuickOrderingSystem.java
java quickorderingsystem.QuickOrderingSystem

