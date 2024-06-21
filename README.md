# HR-Query-App

Effortlessly search and index resumes with the HR Search Application, a powerful tool built using Streamlit. This application allows HR professionals to perform keyword searches on resumes, providing a secure and user-friendly interface for managing and accessing candidate information.

**Features**
- Secure user login with password hashing.
- Index resumes stored in a specified directory.
- Keyword search with support for partial matching.
- Display previews of matching resumes.
- User-friendly interface for seamless navigation.
**Technologies Used**
- Python
- Streamlit
- Whoosh (for indexing and searching)
- PyMuPDF (fitz) (for PDF text extraction)
- SQLite (for user authentication)
**How it Works?**
- User Input
  Login and SignUp: Users can create an account and log in securely using hashed passwords. 
  Keyword Search: Users input keywords (separated by spaces or commas) to search within the indexed resumes.
- Resume Indexing
- PDF Text Extraction: The application extracts text from PDF resumes using PyMuPDF.
- Index Creation: Resumes are indexed using Whoosh, enabling efficient and fast search capabilities.
- Search Functionality
  Keyword Parsing: The input keywords are split and processed to support partial matching.
  Search Execution: The Whoosh searcher executes the search query and returns matching results.
- Result Display: The application displays filenames and text previews of the matching resumes.
**CODE OVERVIEW**
**Libraries Used**
- Streamlit: For creating the web application interface.
- Whoosh: For indexing and searching resume content.
- PyMuPDF (fitz): For extracting text from PDF files.
- SQLite: For managing user authentication.
- Hashlib: For hashing passwords.
**Key Functions**
- User Authentication:

  create_table(): Creates a table for storing user credentials.
  add_data(username, password): Adds a new user to the database.
  login_user(username, password): Validates user login.
  make_hashes(password): Hashes the user's password.
  check_hashes(password, hashed_text): Checks if the input password matches the stored hashed password.
-PDF Text Extraction:
  extract_text_from_pdf(pdf_path): Extracts text from a given PDF file.
-Resume Indexing:
  index_resumes(directory): Indexes resumes from the specified directory using Whoosh.
-Resume Search:
  search_resumes(query): Searches the indexed resumes using the input query with support for partial matching.
- User Interface
  Login and SignUp Pages: Users can log in or create a new account.
  Home Page: Allows logged-in users to search for resumes by entering keywords.
  Search Results: Displays the filenames and previews of the resumes matching the search criteria.
- Skills Required
  Python Programming: Understanding of Python for backend logic and data processing.
  Web Development with Streamlit: Building user interfaces and handling user interactions.
  Database Management: Using SQLite for storing and managing user credentials.
  Text Processing: Extracting and processing text from PDF files.
  Information Retrieval: Using Whoosh for indexing and searching text data.
**Summary**
The HR Search Application simplifies the process of managing and searching resumes for HR professionals. With a secure login system, efficient text extraction, and powerful search capabilities, this tool enhances productivity and makes candidate information easily accessible.
