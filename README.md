# Library-Managment-System
from library import display_all_books, add_book, issue_book, return_book, search_book

print("\n  ======= Welcome to Library Management System =======")

while True:
    print("\n  ----------- MAIN MENU -----------")
    print("  1. Display All Books")
    print("  2. Add New Book")
    print("  3. Issue Book")
    print("  4. Return Book")
    print("  5. Search Book")
    print("  6. Exit")
    print("  ---------------------------------")

    choice = input("  Enter your choice (1-6): ").strip()

    if choice == "1":
        display_all_books()

    elif choice == "2":
        add_book()

    elif choice == "3":
        issue_book()

    elif choice == "4":
        return_book()

    elif choice == "5":
        search_book()

    elif choice == "6":
        print("\n  Thank you for using Library Management System. Goodbye!\n")
        break

    else:
        print("\n  Invalid choice. Please select between 1 and 6.")
