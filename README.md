# Payment Gateway Application

PaymentApp is a Next.js-based payment gateway frontend focused on the customer checkout and payment journey.

The application provides the customer-facing flow for initiating a payment, completing the payment process, and displaying the resulting payment status.

## Customer Payment Journey

The customer payment flow covers:

1. **Checkout Initiation**

   * Displays the payment request and transaction information.
   * Allows the customer to proceed with payment.

2. **Payment Fulfillment**

   * Provides the payment interface.
   * Handles the available payment interaction and processing states.

3. **Verification & Confirmation**

   * Displays the resulting payment status.
   * Supports payment outcomes including:

     * Successful payment
     * Failed payment
     * Pending payment
     * Retry flow
     * Expired or abandoned payment states

The frontend is designed to work with the project's existing payment backend and should not be treated as a replacement for the backend payment services.

## Technology Stack

* **Next.js 14**
* **React 18**
* **TypeScript**
* **Tailwind CSS**
* **Lucide React**

## Requirements

Before running the project, make sure you have:

* Node.js installed
* npm installed

Check your installed versions with:

```bash
node --version
npm --version
```

## Installation

Clone the repository and move into the project directory:

```bash
git clone git@github.com:iBotayo/paymentapp.git
cd paymentapp
```

Install the project dependencies:

```bash
npm install
```

## Development

Start the Next.js development server:

```bash
npm run dev
```

The application runs on:

```text
http://localhost:3005
```

The development server automatically reloads when supported source files are changed.

## Production Build

Create a production build with:

```bash
npm run build
```

After the build completes, start the production server with:

```bash
npm start
```

The production application runs on:

```text
http://localhost:3005
```

## Available npm Scripts

| Command             | Description                                          |
| ------------------- | ---------------------------------------------------- |
| `npm install`       | Installs project dependencies                        |
| `npm run dev`       | Starts the Next.js development server on port 3005   |
| `npm run build`     | Creates a production build                           |
| `npm start`         | Starts the production Next.js server on port 3005    |
| `npm run lint`      | Runs the project's Next.js lint command              |
| `npm run typecheck` | Runs TypeScript type checking without emitting files |

## Project Scope

This repository contains the frontend application for the payment gateway customer experience.

The frontend is responsible for presenting the customer payment journey and its associated payment states. Payment processing, transaction persistence, verification, and other backend responsibilities remain dependent on the project's backend implementation.

## Development Notes

When extending the customer payment journey:

* Preserve the existing application design and styling.
* Reuse existing components and patterns where possible.
* Keep payment states consistent across the checkout flow.
* Do not introduce undocumented or fabricated backend API endpoints.
* Keep sensitive payment information out of client-side logs and source code.
* Verify both successful and unsuccessful payment flows when making changes.

## License

No license has been specified for this project.
