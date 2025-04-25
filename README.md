# BILL.COM

## Overview

BILL.COM is a React-based web application designed for efficient steel billing and invoicing, specifically tailored for small to medium-sized enterprises in the steel industry. Built with TypeScript and styled using Tailwind CSS, this project enables users to create, manage, and print professional invoices with detailed item entries (size, weight, pieces, quantity, rate, total) and automated GST (CGST and SGST) calculations. The application generates downloadable and printable PDFs with a polished layout, leveraging jsPDF, and includes local storage for persistent bill data.

This project combines functionality with a modern, responsive user interface, making it an ideal solution for streamlining billing workflows in steel businesses.
![Landing Page](https://github.com/user-attachments/assets/63562ac5-4f9b-4cf1-879d-1111dd32eb3c)  
*Image 1: The landing page of BILL.COM, showcasing the initial interface with options to create a new bill or edit existing ones, featuring a clean design with a header, input fields for bill details, and action buttons (Save, Download, Print).*

![Bill Creation](https://github.com/user-attachments/assets/5824a013-c43b-4e24-9658-511e706852af)  
*Image 2: The bill creation process, displaying the interactive table where users can add or remove items (e.g., size, quantity, rate), view real-time calculations, and manage bill details like vehicle number and date, highlighting the dynamic and user-friendly interface.*

![PDF Print](https://github.com/user-attachments/assets/4aa76ae5-24cd-4d95-a69f-0be58a461e5d)  
*Image 3: The PDF print output after clicking "Print," showing a professional invoice layout with bill details, an itemized table (e.g., 8mm, 15mm, 12mm items), and a summary section including Total Qty, Avg. Rate, Subtotal, GST, and Grand Total, demonstrating the polished design.*



## Features

- **Responsive Interface**: A mobile-friendly UI built with Tailwind CSS for seamless use across devices.
- **Dynamic Billing**: Add or remove items with real-time updates to quantities, rates, and totals.
- **Automated Calculations**: Computes subtotals, GST (9% CGST & SGST), total quantity, average rate, and grand total.
- **PDF Generation**: Download or print professional invoices with a structured layout using jsPDF.
- **Local Storage**: Save and retrieve bills locally for easy access and editing.
- **Type-Safe Code**: Developed with TypeScript for robust and maintainable code.

## Tech Stack

- **Frontend**: React, TypeScript
- **Styling**: Tailwind CSS
- **PDF Generation**: jsPDF
- **Utilities**: date-fns, lucide-react, uuid
- **Storage**: LocalStorage API

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/bill-com.git
   cd bill-com

## Install Dependencies: Ensure you have Node.js installed, then run:

npm install


## Start the Development Server:

npm start
Open [http://localhost:5173/](http://localhost:5173/) in your browser to view the app.


## Build for Production:

npm run build
This generates a production-ready build in the build folder.


## USAGE
Create a New Bill: Enter bill details (Bill No, Vehicle No, Series, Date) and add items with size, quantity, rate, etc.
Save the Bill: Click "Save" to store the bill locally.
Download/Print: Use "Download" or "Print" to generate a PDF invoice.
Edit Existing Bill: Load a saved bill by ID and modify as needed.
The main component for creating and editing bills. It manages the state of bill details (vehicle number, series, bill number, date, organization name) and items, and handles saving, downloading, and printing bills. It uses useEffect to recalculate totals and GST dynamically.


## Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch: git checkout -b feature/your-feature.
Make your changes and commit: git commit -m "Add your message".
Push to the branch: git push origin feature/your-feature.
Open a Pull Request with a description of your changes.
Please ensure your code follows the existing style and includes appropriate tests or documentation.

## Issues
If you encounter bugs or have feature requests, please open an issue on the GitHub Issues page.

## License
This project is licensed under the MIT License. See the  file for details [LICENSE.md](https://github.com/shivamjoshtech/BILL.COM/blob/main/LICENSE.md) .

## Acknowledgements
Thanks to the open-source communities of React, Tailwind CSS, and jsPDF for their powerful tools.
Inspired by the need for efficient billing solutions in the steel industry.

## Contact
For questions or support, reach out via the GitHub repository: [shivamjoshtech](https://github.com/shivamjoshtech/) or email: joshishivam586@gmail.com.




