# BILL.COM

## Overview

BILL.COM is a React-based web application designed for efficient steel billing and invoicing, specifically tailored for small to medium-sized enterprises in the steel industry. Built with TypeScript and styled using Tailwind CSS, this project enables users to create, manage, and print professional invoices with detailed item entries (size, weight, pieces, quantity, rate, total) and automated GST (CGST and SGST) calculations. The application generates downloadable and printable PDFs with a polished layout, leveraging jsPDF, and includes local storage for persistent bill data.

This project combines functionality with a modern, responsive user interface, making it an ideal solution for streamlining billing workflows in steel businesses.

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

##Install Dependencies: Ensure you have Node.js installed, then run:

npm install


##Start the Development Server:

npm start
Open [http://localhost:5173/](http://localhost:5173/) in your browser to view the app.


##Build for Production:

npm run build
This generates a production-ready build in the build folder.


##USAGE
Create a New Bill: Enter bill details (Bill No, Vehicle No, Series, Date) and add items with size, quantity, rate, etc.
Save the Bill: Click "Save" to store the bill locally.
Download/Print: Use "Download" or "Print" to generate a PDF invoice.
Edit Existing Bill: Load a saved bill by ID and modify as needed.
File Structure


##REPOSITORY TREE

bill-com/

├── src/
│   ├── components/         # React components (BillHeader, BillTable, BillSummary, BillForm)
│   │   ├── BillForm.tsx
│   │   ├── BillHeader.tsx
│   │   ├── BillTable.tsx
│   │   └── BillSummary.tsx
│   ├── types/             # TypeScript interfaces (Bill, BillItem)
│   │   └── index.ts
│   ├── utils/             # Utility functions (calculations, pdfGenerator, storage)
│   │   ├── calculations.ts
│   │   ├── pdfGenerator.ts
│   │   └── storage.ts
│   ├── App.tsx            # Main app component
│   └── index.tsx          # Entry point
├── public/                # Static assets
├── package.json           # Project dependencies and scripts
└── README.md              # This file
└── LICENSE.md             # The License of Copy Rights

##Project Details

BillForm.tsx


The main component for creating and editing bills. It manages the state of bill details (vehicle number, series, bill number, date, organization name) and items, and handles saving, downloading, and printing bills. It uses useEffect to recalculate totals and GST dynamically.

##BillTable.tsx
A component for displaying and editing bill items in a table format. Users can add/remove rows, input item details (size, weight, pieces, quantity, rate), and see calculated totals. Features a responsive design with Tailwind CSS and includes a bin icon for removing items.

##calculations.ts
Handles all billing calculations, including item totals (based on pieces, quantity, and rate), total quantity, average rate, GST (CGST and SGST), and grand total. Ensures accurate financial computations for the bill.

pdfGenerator.ts
Generates PDFs for downloading and printing bills using jsPDF. Produces a professional, responsive layout with a header (organization name, invoice title), bill details, item table, and summary section (total quantity, average rate, subtotal, GST, grand total). Supports pagination for long item lists.

storage.ts
Manages bill persistence using LocalStorage. Provides functions to save, retrieve, and delete bills, ensuring all bill data (including items and calculations) is stored securely and can be retrieved for editing.

Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch: git checkout -b feature/your-feature.
Make your changes and commit: git commit -m "Add your message".
Push to the branch: git push origin feature/your-feature.
Open a Pull Request with a description of your changes.
Please ensure your code follows the existing style and includes appropriate tests or documentation.

Issues
If you encounter bugs or have feature requests, please open an issue on the GitHub Issues page.

License
This project is licensed under the MIT License. See the  file for details.

Acknowledgements
Thanks to the open-source communities of React, Tailwind CSS, and jsPDF for their powerful tools.
Inspired by the need for efficient billing solutions in the steel industry.

Contact
For questions or support, reach out via the GitHub repository or email: joshishivam586@gmail.com.




