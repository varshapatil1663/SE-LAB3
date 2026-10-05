# Lab 3: Component Modelling & Architectural Pattern Selection

## Self-Service Coffee Kiosk System

### Objective

The objective of this lab is to evaluate different architectural styles, select an appropriate architecture for the given system, and create a UML Component Diagram showing the system components, interfaces, and dependencies.

## System Description

The system is a **Self-Service Coffee Kiosk** that allows customers to:

* Select coffee from three options:

  * Espresso
  * Americano
  * Latte
* Select the size:

  * Small
  * Large
* Make payment using a credit card.
* Receive a printed receipt.

The system uses a touchscreen interface, receipt printer, and menu/pricing storage.

## Selected Architecture

**Layered Architecture** was selected for the Self-Service Coffee Kiosk System.

Layered Architecture provides clear separation of responsibilities between the user interface, business logic, payment processing, data storage, and hardware interaction.

## Components

The UML Component Diagram contains the following five components:

1. **Touchscreen Interface** – Handles customer interaction and order selection.
2. **Order Manager** – Processes and manages customer orders.
3. **Payment Service** – Handles credit-card payment processing.
4. **Menu Database** – Stores coffee menu and pricing information.
5. **Receipt Printer** – Prints the receipt after a successful order.

## Interfaces and Communication

The major interfaces between the components include:

* **Order Service** – Communication between the Touchscreen Interface and Order Manager.
* **Payment Processing** – Communication between the Order Manager and Payment Service.
* **Menu Data Access** – Communication between the Order Manager and Menu Database.
* **Receipt Printing** – Communication between the Order Manager and Receipt Printer.

The diagram uses UML provided and required interface notation where applicable.

## Architecture Justification

Layered Architecture was selected because it provides separation of responsibilities. The Touchscreen Interface handles user interaction, while the Order Manager handles order processing. The Payment Service manages payments, and the Menu Database manages menu and pricing information.

This architecture also makes it easier to manage the kiosk's hardware and data separately. The receipt printer can be handled independently from the menu database and payment processing.

From a security perspective, separating the Payment Service from the user interface helps isolate sensitive payment processing.

From a performance perspective, each component performs a specific responsibility, reducing unnecessary processing and allowing requests to be handled efficiently.

## Deliverables

* UML Component Diagram – PNG/PDF
* Architecture Justification – PDF
* README.md

## Tools Used

* **draw.io** – UML Component Diagram
* **GitHub** – Repository and submission
* **Layered Architecture** – Selected architectural style

## Conclusion

The Self-Service Coffee Kiosk System is modelled using a Layered Architecture with five major components and their corresponding interfaces. The architecture provides separation of responsibilities, easier maintenance, security benefits, and efficient processing.
