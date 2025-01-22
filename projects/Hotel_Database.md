---
layout: project
type: project
image: img/hotelresized.jpg
title: "Hotel Booking System Simulator"
date: 2023
published: true
labels:
  - Database
  - Simulation
  - C++
summary: "My team and I created a C++ program to simulate a hotel booking system."
---

In my programming structures class, I worked on a team of six students to create and implement a simulation of a system that mirrors software used in the hotel industry. This simulator included functionality such as
searching, adding, deleting, and updating rooms. Alongside this, the simulator could also gather customer data and check them in/out of rooms.

Personal duties on this project include:
- Pulling customer/room details from the booking database for a "Guest Summary" function
- Implementing a search function for rooms in the database

## Source code for guest summary function: 
```
    void printGuestSummary(vector<Customer>& customers) {
      for (int i = 0; i < customers.size(); i++) {
        customers[i].displayCustomerDetails();
        cout << "\n";
      }
      if(customers.size() == 0){
        cout << "There are no guests.";
      }
      cout << "\n";
    }

```
## Source code for search function:

```
void searchRoom(vector<Room>& rooms) {
      int roomNum;
      cin.ignore();
      cout << "\nEnter Room Number: ";
      cin >> roomNum;
      cin.ignore();

      bool roomFound = false;  // Flag to check if the room is found
      for (int i = 0; i < rooms.size(); i++) {
          if (rooms[i].getRoomNumber() == roomNum) {
              roomFound = true;  // Set the flag to true if the room is found
              cout << "Room Details" << endl;
              if (rooms[i].getAvailability()) {
                  cout << "\nRoom is available" << endl;
              } else {
                  cout << "\nRoom is not available" << endl;
              }

              cout << "Room Number: " << rooms[i].getRoomNumber() << endl;
              cout << "Type AC/No AC (A/N) " << rooms[i].getType() << endl;
              cout << "Comfort (S/N) " << rooms[i].getComfort() << endl;
              cout << "Size (B/S) " << rooms[i].getSize() << endl;
              cout << "Daily Rate: " << rooms[i].getDailyRate() << endl;
              break;
          }
      }

      // Print the "not found" message only if the room is not found
      if (!roomFound) {
          cout << "\nRoom does not exist, try again." << endl;
      }
  } 

```
