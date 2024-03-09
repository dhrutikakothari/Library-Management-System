
# Library Management System (LMS)

## Overview
The Library Management System (LMS) is a Java-based application designed to streamline the management of books within a library. This user-friendly system allows librarians or administrators to perform various tasks related to book management. The application follows a fundamental MVC (Model-View-Controller) architecture, dividing responsibilities among the model, view, and controller components.

## Model
- Represents the application's data and business logic.
- Manages data, logic, and rules of the application.
- Encapsulates the state and behavior of the application.
- Independent of the user interface; no direct interaction with the presentation layer.

## View
- Represents the user interface and presentation layer.
- Displays data to the user and captures user input.
- Receives user input and sends commands to the controller.
- Responsible for presenting data and receiving user interactions, with minimal knowledge of the underlying application logic.

## Controller
- Acts as an intermediary between the model and the view.
- Handles user input and updates the model accordingly.
- Orchestrates the flow of data between the model and the view.
- Contains the application's business logic, governing how data is processed and presented.
  ![image](https://github.com/dhrutikakothari/Library-Management-System/assets/161920429/119e5d2e-f68f-4438-9709-38dd75cde7d8)
  
# Benefits of MVC Architecture

The Library Management System (LMS) employs the Model-View-Controller (MVC) architecture, providing several advantages for the development and maintenance of the application.

## Key Benefits:

### 1. Separation of Concerns:
- MVC enforces a clear separation of concerns, ensuring that each component (Model, View, Controller) has a specific and well-defined role.
- This separation simplifies code maintenance and modification.

### 2. Modularity and Reusability:
- The modular structure of MVC allows for independent development and testing of each component (Model, View, Controller).
- Models, views, and controllers can be reused in different parts of the application or other projects, promoting code reusability.

### 3. Scalability:
- MVC provides a scalable architecture that supports the addition or modification of features without affecting other parts of the application.
- New functionalities can be added by introducing new controllers, views, or models, maintaining the integrity of existing code.

### 4. Maintainability:
- The separation of concerns and modularity contribute to better code maintainability.
- Changes in one component (e.g., updating business logic) do not require modifications to other components, reducing the risk of unintended side effects.

### 5. Ease of Testing:
- Each component in MVC can be tested independently, making it easier to identify and fix bugs.
- Automated testing of models, views, and controllers ensures that each part of the application functions correctly in isolation.

### 6. Flexibility:
- MVC allows developers to choose different technologies for each component. For example, the same model could be used with different views or controllers.

### 7. Enhanced Collaboration:
- MVC promotes collaborative development as different teams or developers can work on different components simultaneously.
- The clear separation of concerns facilitates collaboration by minimizing dependencies between components.


## Classes and Packages

### Library Class

**Package Name:**
- com.jsp.lms.model

**Attributes (Fields):**
1. `libraryName` (Type: String)
2. `libraryAddress` (Type: String)
3. `pincode` (Type: int)
4. `books` (Type: List<Book>)

**Methods:**
- `getLibraryName():` Returns the libraryName.
- `setLibraryName(String libraryName):` Sets the libraryName.
- `getLibraryAddress():` Returns the libraryAddress.
- `setLibraryAddress(String libraryAddress):` Sets the libraryAddress.
- `getPincode():` Returns the pincode.
- `setPincode(int pincode):` Sets the pincode.
- `getBooks():` Returns the books.
- `setBooks(List<Book> books):` Sets the books.

### Book Class

**Package Name:**
- com.jsp.lms.model

**Attributes (Fields):**
1. `bookName` (Type: String)
2. `bookAuthor` (Type: String)
3. `bookPrice` (Type: double)

**Methods:**
- `getBookName():` Returns the bookName.
- `setBookName(String bookName):` Sets the bookName.
- `getBookAuthor():` Returns the bookAuthor.
- `setBookAuthor(String bookAuthor):` Sets the bookAuthor.
- `getBookPrice():` Returns the bookPrice.
- `setBookPrice(double bookPrice):` Sets the bookPrice.
- `toString():` Overrides the toString method.

### View Class

**Package Name:**
- com.jsp.lms.view

**Attributes (Fields):**
1. `library` (Type: Library)
2. `myInput` (Type: Scanner)
3. `controller` (Type: Controller)

**Methods:**
- `getLibrary():` Returns the library.
- `setLibrary(Library library):` Sets the library.
- `main(String[] args):` The main method containing program logic.

### Controller Class

**Package Name:**
- com.jsp.lms.controller

**Attributes (Fields):**
1. `library` (Type: Library)

**Methods:**
- `addBook(Book book):` Adds a book to the library.
- `getBook(String bookName):` Retrieves a book from the library.
- `update(Book bookExist, Book bookUpdate):` Updates book details.
- `removeBook(String bookName):` Removes a book from the library.

## User Guide

### 1. Application Initialization:

Upon launching the application, the user is prompted to enter essential details about the library, including the name, address, and pincode. These details are captured during the static initialization block in the View class.




