Assignment                                                                                                                                           2026-10-18 

**Name:** Ali Salaheldeen Adam Tour **Email:** <u>sultanalitaaru911@gmail.com</u> 

**Institution:** Kigali Independent University (ULK) 

# **SMART HOSTEL MANAGEMENT SYSTEM** 



<!-- Start of picture text -->
Admin<br>~ adminid: int<br>~fullName: String<br>emai: String<br>+ manageRooms(): void a)<br>+ manageBookings(): void<br>+ ViewPayments(): void<br>Customer Room<br>~ customerig: int ~roomid: int<br>~fullName: String ~roomNumber: String<br>= email String = roomType: String<br>+phone:register():Stringvoid oroneee TOT 7 rice: double<br>+ +makePayment():bookRoom(): voidvoid feserved thrdjugh (1 0.*) + checkAvaitabilty(:+ updatestatus0) booleanvoid<br>submits(1: 0."<br>smakes(1: 0." handles(1 0.*)<br>makes(1: 0.*) ~bookingld:Booking int MaintenanceRequest~requestid: int<br>- bookingDate: Date - description: String<br> checkinDate: Date ~requestDate: Dale<br>~ checkOutDate:~ status: String Date = status: String<br>+ submitRequest(): void<br>+ createBooking(): void + updateStatus(): void<br>+ cancelBooking(): void<br>as (10.|<br>Payment<br>~paymentid: int<br>~ amount: double<br>~paymentDate: Date<br>- paymentMethod: String<br>~ status: String<br>+ processPaymenti): void<br>+ generateReceipt(): void<br><!-- End of picture text -->

## **1. Introduction** 

A UML class diagram represents the structure of a software system by showing its classes, attributes, methods, and relationships. The class diagram for the Smart Hostel Management System contains six main classes: Customer, Admin, Room, Booking, Payment, and MaintenanceRequest. 

## **2. Classes, Attributes, and Methods** 

## **2.1 Customer** 

**Attributes:** customerId, fullName, email, phone 

**Methods:** register(), bookRoom(), makePayment() 

**Responsibility:** Manages customer information and customer activities. 

## **2.2 Admin** 

**Attributes:** adminId, fullName, email 

**Methods:** manageRooms(), manageBookings(), handleMaintenance() 

**Responsibility:** Oversees hostel operations. 

## **2.3 Room** 

**Attributes:** roomId, roomNumber, roomType, price, status 

**Methods:** checkAvailability(), updateStatus(), updatePrice() 

**Responsibility:** Stores room information and manages availability. 

## **2.4 Booking** 

**Attributes:** bookingId, customerId, roomId, bookingDate, checkInDate, checkOutDate, status 

**Methods:** createBooking(), cancelBooking(), updateBooking() 

**Responsibility:** Manages room reservations and booking details. 

## **2.5 Payment** 

**Attributes:** paymentId, bookingId, customerId, amount, paymentDate, paymentMethod, status 

**Methods:** processPayment(), verifyPayment(), generateReceipt() 

**Responsibility:** Records and tracks customer payments. 

## **2.6 MaintenanceRequest** 

**Attributes:** requestId, customerId, roomId, description, requestDate, status, handledBy 

**Methods:** submitRequest(), updateStatus(), assignAdmin() 

**Responsibility:** Records maintenance problems and tracks their resolution. 

## **3. Relationships and Multiplicities** 

**Relationship Multiplicity Explanation** 

One customer can make multiple bookings; each booking belongs Customer — Booking 1 to 0..* to one customer. 

|**Relationship**|**Multiplicit i**|**iy Explanation**|
|---|---|---|
|Room — Booking|1 to 0..*|One room can have multiple bookings over time; each booking<br>refers to one room.|
|Booking — Payment|1 to 0..*|One booking can have multiple payment records; each payment<br>belongs to one booking.|
|Customer — Payment|1 to 0..*|One customer can have multiple payment records; each payment<br>belongs to one customer.|
|Customer —<br>MaintenanceRequest|1 to 0..*|One customer can submit multiple maintenance requests; each<br>request belongs to one customer.|
|Room —<br>MaintenanceRequest|1 to 0..*|One room can have multiple maintenance requests; each request<br>concerns one room.|
|Admin — Room|1 to 0..*|One administrator can manage multiple rooms.|
|Admin — Booking|1 to 0..*|One administrator can oversee multiple bookings.|
|Admin —<br>MaintenanceRequest|1 to 0..*|One administrator can handle multiple maintenance requests.|



**Multiplicity notation:** 

- 1 means exactly one. 

- 0..* means zero, one, or many. 

## **4. Explanation of the Relationships** 

The Customer class is connected to Booking, Payment, and MaintenanceRequest because customers can reserve rooms, make payments, and report maintenance problems. 

The Room class is connected to Booking and MaintenanceRequest because rooms can be reserved and may require repairs. 

The Booking class is connected to Payment because payments are recorded against bookings. A booking may have no payments or several payment records. 

The Admin class is connected to Room, Booking, and MaintenanceRequest because administrators manage rooms, oversee reservations, and handle maintenance issues. 

These relationships show how the different parts of the system interact and help guide the design of the PostgreSQL database. 

## **5. Conclusion** 

The UML class diagram provides a structural representation of the Smart Hostel Management System. It identifies the six main classes, their attributes and methods, and the relationships between them. The diagram also serves as a guide for implementing the database and organizing the system's functionality. 

