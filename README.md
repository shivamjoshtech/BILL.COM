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
