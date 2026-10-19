# Admin
## Attributes
- adminId: int
- fullName: String
- email: String
## Methods
+ manageRooms(): void
+ manageBookings(): void
+ viewPayments(): void

# Customer
## Attributes
- customerId: int
- fullName: String
- email: String
- phone: String
## Methods
+ register(): void
+ bookRoom(): void
+ makePayment(): void

# Room
## Attributes
- roomId: int
- roomNumber: String
- roomType: String
- price: double
- status: String
## Methods
+ checkAvailability(): boolean
+ updateStatus(): void

# Booking
## Attributes
- bookingId: int
- bookingDate: Date
- checkInDate: Date
- checkOutDate: Date
- status: String
## Methods
+ createBooking(): void
+ cancelBooking(): void

# MaintenanceRequest
## Attributes
- requestId: int
- description: String
- requestDate: Date
- status: String
## Methods
+ submitRequest(): void
+ updateStatus(): void

# Payment
## Attributes
- paymentId: int
- amount: double
- paymentDate: Date
- paymentMethod: String
- status: String
## Methods
+ processPayment(): void
+ generateReceipt(): void