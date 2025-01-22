---
layout: project
type: project
image: img/library.jpg
title: "Library Database Simulator"
date: 2023
published: true
labels:
  - Database
  - Simulation
  - C++
summary: "My team and I created a C++ program to simulate a library database system."
---
As part of a mid-term project for my Program Structure class, I worked in a team of six other students to create a simulation of a library database in C++. The main functionality of this system consisted of book indexing via its title/ISBN/genre/author. 
Other important aspects included book searching, adding/deleting, and editing.

Personal duties on this project include:
- Implementing an "edit book" feature
- Implementing library database search functionality

## Source Code for edit book feature:
```
void editBook(Book library[], int librarySize)
{
    string searchItem, newValue, oldValue;
    int input;

    cout << "Enter the ISBN of book to be edited: ";
    cin.ignore();
    getline(cin, searchItem);
    for (int i = 0; i < librarySize; i++)
    {
        if (library[i].getISBN() == searchItem)
        {
            cout << "Title: " << library[i].getTitle() << " | ";
            cout << "Author: " << library[i].getAuthor() << " | ";
            cout << "ISBN: " << library[i].getISBN() << " | ";
            cout << "Edition: " << library[i].getEdition() << " | ";
            cout << "Publication: " << library[i].getPublication() << "\n\n";

            cout << "Are you sure you want to edit this book?\n";
            cout << "[1] YES\n"
                 << "[2] NO\n";
            cout << "Enter choice: ";
            cin >> input;
            cout << "\n";
            switch (input)
            {
            case 1:
                while (true) // Loops indefinitely until user indicates they are done editing the book.
                {
                    cout << "[1] Title\n";
                    cout << "[2] Author\n";
                    cout << "[3] ISBN\n";
                    cout << "[4] Edition\n";
                    cout << "[5] Publication\n";
                    cout << "Enter choice: ";
                    cin >> input;
                    cin.ignore();
                    cout << "\n";
                    switch (input)
                    {
                    case 1:
                        oldValue = library[i].getTitle();
                        cout << "Enter new title: ";
                        getline(cin, newValue);
                        library[i].setTitle(newValue);
                        cout << "\nOld title: "
                             << oldValue
                             << " New title: "
                             << library[i].getTitle();
                        cout << "\nTitle successfuly changed!\n";
                        break;
                    case 2:
                        oldValue = library[i].getAuthor();
                        cout << "Enter new author: ";
                        getline(cin, newValue);
                        library[i].setAuthor(newValue);
                        cout << "\nOld author: " << oldValue << " New author: " << library[i].getAuthor();
                        cout << "\nAuthor successfuly changed!\n";
                        break;
                    case 3:
                        oldValue = library[i].getISBN();
                        cout << "Enter new ISBN: ";
                        getline(cin, newValue);
                        library[i].setISBN(newValue);
                        cout << "\nOld ISBN: " << oldValue << " New ISBN: " << library[i].getISBN();
                        cout << "\nISBN successfuly changed!\n";
                        break;
                    case 4:
                        oldValue = library[i].getEdition();
                        cout << "Enter new edition: ";
                        getline(cin, newValue);
                        library[i].setEdition(newValue);
                        cout << "\nOld edition: " << oldValue << " New edition: " << library[i].getEdition();
                        cout << "\nEdition successfuly changed!\n";
                        break;
                    case 5:
                        oldValue = library[i].getPublication();
                        cout << "Enter new publication: ";
                        getline(cin, newValue);
                        library[i].setPublication(newValue);
                        cout << "\nOld publication: " << oldValue << " New publication: " << library[i].getPublication();
                        cout << "\nPublication successfuly changed!\n";
                        break;
                    }
                    cout << "Keep editing?\n";
                    cout << "[1] YES\n"
                         << "[2] NO\n";
                    cout << "Enter choice: ";
                    cin >> input;
                    switch (input)
                    {
                    case 1:
                        break; // breaks the switch and starts at the begining of the while loop
                    case 2:
                        return; // exits function
                    }
                }
            case 2:
                return;
            }
        }
    }
    cout << "\nNo book with this ISBN found.";
    cout << "\n----------------------------------------\n";
}

```

## Source Code for search feature:
```
void searchBook(Book library[], int librarySize)
{
    string searchItem; // value to be searched for in library
    cout << "Search by title, author, or ISBN: ";
    cin.ignore();
    getline(cin, searchItem);
    cout << "\n--------- Search results ---------\n";
    for (int i = 0; i < librarySize; i++)
    { // loops through array, if either title or author or ISBN match user input, prints all instances of those books
        if (library[i].getTitle() == searchItem || library[i].getAuthor() == searchItem || library[i].getISBN() == searchItem)
        {
            cout << "Title: " << library[i].getTitle() << " | ";
            cout << "Author: " << library[i].getAuthor() << " | ";
            cout << "ISBN: " << library[i].getISBN() << " | ";
            cout << "Edition: " << library[i].getEdition() << " | ";
            cout << "Publication: " << library[i].getPublication() << "\n\n";

        }
    }
    cout << "\n----------------------------------------\n";
}

```

