# MSc Project 1 - Lending Library
I was tasked with developing an object-oriented library system that simulates notifications for library members. The system was designed with extensibility in mind, enabling future requirements to be added without substantial changes. The task involved handling loans, returns, membership and notification systems using CSV/JSON files for storage.
Tasks Breakdown:

1. Task 1: Convert CSV Files to JSON Files
   - Objective: I had to convert the provided `books_2024.csv`, `bookloans_2024.csv`, and `members_2024.csv` files into JSON format.
   - Requirements:
     - I needed to implement the `scan()` method in the `Book` and `Member` classes to simulate the scanning of a book or membership card.
     - Then I needed to update the JSON file when a member borrows a book.
     - Testing: I used dummy data to test the borrowing operation and included preconditions and postconditions in a docstring.

2. Task 2: Implement Book Return Functionality
   - Objective: I needed to allow members to return books and then update the JSON files accordingly.
   - Requirements:
     - I had to update the JSON file when a book was returned.
     - Testing: I used dummy data to test the return operation and included preconditions and postconditions in a docstring.
     - Note: if a book was reserved, a notification of its availability was required.

3. Task 3: Membership Application and Card Issuance System
   - Objective was to create a system that managed membership applications and the issuance of membership cards along with unique number identifiers.
   - Requirements:
     - To implement a format for membership card numbers (e.g., `ID-1`, `ID-2`).
     - To handle card reissuance, ensuring unique and non-duplicated card numbers.
     - To reset card issuance count after 99 cards have been issued.
     - To update the JSON membership file to reflect card issuance and reissuance transactions.

4. Task 4: Implement Book Reservation System
   - The objective was to provide functionality for members to be able to reserve books and manage their availability.
   - Requirements:
     - To allow members to reserve books.
     - I had to create a new `reserved.json` file to store reservation data.
     - To issue a notification when a reserved book becomes available.

5. Task 5: Implement Notification System
   - The objective was provide a flexible notification system for various library events.
   - Requirements:
     - The system needed to notify members when a reserved book becomes available.
     - It needed to notify members if they returned a book late, and include the fine amount.
     - Extensibility: I needed to consider the system's ability to accommodate future notification requirements.
     - The Handling of CSV and JSON files needed to be efficient and seemless.

 Design and Documentation:
- Classes: I needed to implement at least two custom classes (`Book` and `Member`), with a likely additional `Library` class to manage books, members, loans, reservations, and notifications.
- Design Patterns: I had to utilize design patterns to ensure the system is extensible and maintainable.
- Documentation: I included docstrings and markdown cells explaining my design choices, the handling of CSV/JSON files, and reflections on the extensibility of my notification system.
