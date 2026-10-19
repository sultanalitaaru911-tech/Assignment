Assignment 

2026-10-18 

**Name:** Ali Salaheldeen Adam Tour 

**Email:** sultanalitaaru911@gmail.com 

**Institution:** Kigali Independent University (ULK) 

# **Project Title: Smart Hostel Management System** 

## **1. System Description** 

The Smart Hostel Management System manages hostel operations, including customer registration, room allocation, bookings, payments, and maintenance requests. It allows administrators to manage rooms and monitor payments while customers can book rooms and report maintenance problems. 

## **2. Explanation of the Classes** 

|**Class**|**Description**|
|---|---|
|**Customer**|Stores customer information and allowscustomerstobook rooms, make<br>payments, and submit maintenance requests.|
|**Admin**|Manages hostel rooms, oversees bookings, monitors payments,and<br>handles maintenance requests.|
|**Room **|Stores room details, including roomnumber, type,price,and availability<br>status.|
|**Booking**|Records room reservations,bookingdates, check-in dates, check-out<br>dates, and bookingstatus.|
|**Payment**|Records paymentamounts,paymentdates,payment methods,and<br>payment status.|
|**Maintenance**|Stores maintenanceproblemsreported bystudents andtrackstheir|
|**Request**|resolution.|



## **3. Relationships Between Classes** 

**1. Customer and Booking — One-to-Many (1 to 0..*)** 

One customer can make multiple bookings, but each booking belongs to one customer. 

**2. Room and Booking — One-to-Many (1 to 0..*)** 

A room can be associated with multiple bookings over time, but each booking refers to one room. The system must prevent conflicting active bookings for the same room. 

**3. Booking and Payment — One-to-Many (1 to 0..*** 

A booking can have multiple payment records, for example, a deposit followed by a balance payment. 

## **4. Customer and Payment — One-to-Many (1 to 0..*)** 

A student can make multiple payments, but each payment is associated with one student. 

## **5. Customer and Maintenance Request — One-to-Many (1 to 0..*)** 

A student can submit multiple maintenance requests, but each request is submitted by one student. 

## **6. Room and Maintenance Request — One-to-Many (1 to 0..*)** 

A room can have multiple maintenance requests over time, but each request concerns one room. 

**7. Admin and Room — One-to-Many (1 to 0..*)** 

One administrator can manage multiple rooms. 

## **8. Admin and Booking — One-to-Many (1 to 0..*)** 

One administrator can oversee multiple bookings. 

**9. Admin and Maintenance Request — One-to-Many (1 to 0..*)** 

One administrator can handle multiple maintenance requests. 

## **4. UML Notation Used** 

Each class contains three sections: 

1. **Class name:** The name of the class, such as csutomer. 

2. **Attributes:** The information stored by the class, such as studentId and fullName. 

3. **Methods:** The operations performed by the class, such as bookRoom() and makePayment(). 

The visibility symbols are: 

- + Public — accessible from other classes. 

- - Private — accessible only within the class. 

- # Protected — accessible within the class and its subclasses. 

The diagram uses + to indicate public attributes and methods for simplicity. In a production implementation, attributes would generally be private, with public methods providing controlled access. 

