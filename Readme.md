# HandsMen Threads CRM

A Salesforce CRM solution for **HandsMen Threads**, a premium men's fashion and tailoring brand. The project brings customer, order, product, inventory, and marketing information together and uses Salesforce automation to support day-to-day operations and customer engagement.

## Project overview

The solution is designed around five Salesforce custom objects:

- **Customer** — customer details and engagement.
- **Order** — order information and order status.
- **Product** — product catalog and pricing.
- **Inventory** — stock levels associated with products.
- **Marketing Campaign** — campaign and marketing activity.

The Salesforce implementation described in the project documentation includes record-triggered and scheduled flows, email alerts, validation rules, and role-based access for Sales, Inventory, and Marketing teams. Apex is used for additional order and inventory logic.

## Key capabilities

- Manage customer, product, order, inventory, and marketing records in one CRM.
- Calculate order totals from product prices and order quantities.
- Deduct inventory when an order is confirmed.
- Automate order confirmations, loyalty updates, and low-stock notifications.
- Apply validation rules to help maintain accurate, consistent records.
- Organize Salesforce access and data visibility for different business teams.

## Demo

[Watch the project demo](https://drive.google.com/file/d/10T9bJ36jqJ90lQo34xKUd2-7DYZviPx-/view)

## Repository contents

| Path | Description |
| --- | --- |
| `HandsMen Threads Project Documentation.docx` | Project objectives, Salesforce design, implementation overview, and future enhancements. |
| `Screenshots/` | Screenshots of the Salesforce app, records, configuration, flows, and email alerts. |
| `source code/` | Text files containing Apex trigger examples for order totals and stock deduction. |

### Apex examples

- [`update order total.txt`](source%20code/update%20order%20total.txt) — calculates an order's total from its quantity and related product price.
- [`Stock Deduction Trigger.txt`](source%20code/Stock%20Deduction%20Trigger.txt) — deducts inventory for confirmed orders.

These are source examples, not a complete Salesforce deployment package. The repository does not include deployable Salesforce metadata or an org configuration. Before using the snippets, verify that the object and field API names match your Salesforce org, and test the automation in a sandbox.

## Screenshots

### Salesforce app and data model

- [HandsMen Threads app navigation](Screenshots/HandsMen%20Threads%20App%20Navigation%20Items.png)
- [Custom object](Screenshots/Custom%20Object.png)
- [Customer records](Screenshots/HandMen%20Customers.png)
- [Create a customer](Screenshots/Creating%20New%20HandMen%20Customer.png)
- [Customer validation](Screenshots/Customer%20validation.png)
- [Product record](Screenshots/Product%20in%20HandMen%20Products.png)
- [Order record](Screenshots/Order%20in%20HandMen%20Orders.png)
- [Roles](Screenshots/Roles.png)
- [User](Screenshots/User%20Niklaus.png)

### Automation and customer communications

- [Order confirmation flow](Screenshots/Order%20confirmation%20flow.png)
- [Order confirmation email](Screenshots/Order%20Confirmed%20Email.png)
- [Low-stock alert flow](Screenshots/Low%20stock%20alert%20flow.png)
- [Low-stock alert email](Screenshots/Low%20stock%20alert%20Email.png)
- [Loyalty program flow](Screenshots/Loyality%20program%20flow.png)
- [Loyalty program email](Screenshots/Loyality%20program%20Email.png)
- [Email alerts overview](Screenshots/All%20Email%20Alerts.png)
- [Classic email template](Screenshots/classic%20email%20template.png)

## Getting started

This repository is a documentation and example-code project; it is not an installable Salesforce package.

1. Review the [project documentation](HandsMen%20Threads%20Project%20Documentation.docx) and screenshots to understand the Salesforce configuration.
2. In a Salesforce sandbox, create or confirm the required objects, fields, relationships, flows, email templates, validation rules, and access settings.
3. Review the Apex examples and update their API names and business logic to match your org.
4. Test the flows and triggers with representative orders and inventory records before deploying changes to production.

## Future enhancements

Potential next steps described in the project documentation include customer portal access, reports and dashboards, mobile access, personalized recommendations, and WhatsApp or SMS notifications.
