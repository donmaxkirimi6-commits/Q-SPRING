# Water Logistics Tracker

A simple web application that tracks water from production to delivery, together with the electricity used, the money coming in, and the money going out. It turns these records into weekly and monthly reports, so the owner can see how much water was produced and delivered, what it cost, and what profit was made.

**Live site:** https://donmaxkirimi6-commits.github.io/Q-SPRING/
*(available once GitHub Pages is switched on for this repository)*

## Features

| Section | What it records or shows |
|---------|--------------------------|
| **Dashboard** | This month's totals: water produced, water delivered, water not delivered, electricity use and cost, income, expenditure, and profit |
| **Production** | Date, litres produced, and source (for example, a borehole) |
| **Delivery** | Date, customer, litres delivered, and vehicle |
| **Electricity** | Date, units used (kWh), and cost (KSh) |
| **Income** | Date, who paid, and the amount (KSh) |
| **Expenditure** | Date, category (fuel, wages, repairs and so on), and the amount (KSh) |
| **Reports** | Weekly and monthly summaries with totals, which can be exported as a CSV file or printed |

Other features:
- Works on phones, tablets, and computers
- Follows the device's light or dark mode
- Includes a **Load sample data** option for trying the system before entering real records
- Needs no installation, server, or internet connection once the page has loaded

## How the figures are calculated

- **Not delivered** = water produced − water delivered. This helps to spot losses, storage, or unrecorded sales.
- **Power per 1,000 L** = electricity used (kWh) ÷ litres produced × 1,000.
- **Profit** = income − expenditure − electricity cost.
- Weekly reports group records by week, and weeks start on Monday.

## How to use it

1. Open the site (or open `index.html` in a browser).
2. Choose a tab, such as **Production**, fill in the form, and click **Add record**.
3. Repeat for delivery, electricity, income, and expenditure.
4. Open **Dashboard** for this month's totals, or **Reports** for weekly and monthly tables.
5. In **Reports**, click **Export CSV** to save a copy, or **Print** to print it.
6. To remove a record, click **Delete** beside it.

## Run it on your computer

No setup is needed:

1. Download or clone this repository.
2. Double-click `index.html` to open it in a web browser.

```
git clone https://github.com/donmaxkirimi6-commits/Q-SPRING.git
```

## Publish it with GitHub Pages

1. Open the repository and go to **Settings**, then **Pages**.
2. Under **Branch**, choose `main` and click **Save**.
3. After a minute or two, the site link appears on the same page.

## Project structure

```
Q-SPRING/
├── index.html     # the whole application (HTML, CSS and JavaScript)
└── README.md      # this file
```

## Built with

- HTML
- CSS
- JavaScript (no frameworks or libraries)

## Important to know

- Records are saved in the **browser on the device being used** (using the browser's local storage). They are not shared between different phones or computers.
- Clearing the browser's site data deletes the records, so use **Export CSV** regularly to keep a copy.
- The amounts are shown in Kenya shillings (KSh).

## Ideas for future improvement

- A database so that several people can enter and view the same records
- User login with different roles (owner, driver, accountant)
- Editing of existing records
- Charts for production, delivery, and profit
- Vehicle and route tracking
- Customer balances and payment reminders

## Author

Donmax Murithi
