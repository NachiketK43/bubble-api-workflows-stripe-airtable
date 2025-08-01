# bubble-api-workflows-stripe-airtable
Bubble.io app showcasing integrations of Bubble with Stripe for subscription payment and Bubble with Airtable for fetching live data from Airtable base

**Feature List**

- User login/signup flow
- Tiered pricing page 
- Stripe Checkout integration (via API Connector)
- Account page 
- Property Listings page 
- Create and edit property listings 

---

## Demo App Link
🔗 [Click to view demo app](https://test-app-58311.bubbleapps.io/version-test/signup_login)

Create an account or use this test account to explore the demo:

- **Email**: olivia.hart@skyline.net
- **Password**: G7r!Kzq2L#t5

⚠️ Data may reset periodically.

---
## API Integrations

### Stripe API
- Create Checkout Session
- Retrieve Subscription
- Retrieve Invoice
- Cancel Subscription

### Airtable API
- Retrieve property listings data from base
- Send records to Bubble and display on page
- Edit/Create property listings

---

## Project Features

**User Login/Signup Flow**
- Enables user to sign up or log in
- Utilized Bubble’s built-in User data type and Authentication actions
- Custom workflows directs user to Pricing Page to select a subscription tier 
<br>

**Tiered Pricing Page with Subscription Plans**
- Displays three transparent pricing tiers: Monthly ($20), Semi-Annual ($100), and Yearly ($170), allowing users to select one
- Upon selection of any one tier, a workflow triggers a call to Stripe Checkout Session API with plan-specific metadata
- User makes the payment and is directed back to the pricing page
<br>

**Stripe Checkout Integration (via API Connector)**
- Directs the user to Stripe’s hosted checkout page for secure card entry and payment
- POST /v1/checkout/session set up to create new subscriptions
- GET /v1/subscriptions and GET /v1/invoices for status/invoice retrieval
<br>

**Account Page with Plan Details**
- Allows users to view their active plan, next billing date, and update account details like name/email
- "Cancel" buttons connect with Stripe via API Connector
<br>
 
 **Listings Page Fetching Data from Airtable**
 - Connected Airtable using Bubble’s API Connector
 - Used Airtable’s GET endpoint to fetch listing records
 - Data is displayed using a Repeating Group, dynamically populated from the Airtable response
 - Each listing card includes edit/delete icons that trigger corresponding Airtable updates
 
    
---
## Screenshots

### Listing Page
![Listing Page](screenshots/Create%20Listing%20Page.png)


### Account Page (Bubble Editor
![Account Page (Bubble Editor)](screenshots/Account%20Page%20(Bubble%20Editor).png)


### Account Page
![Account Page](screenshots/Account%20Page.png)


### Airtable Base
![Airtable Base](screenshots/Airtable%20Base%20.png)


### Airtable Workflow – Creating a New Listing
![Airtable Workflow – Creating a New Listing](screenshots/Airtable%20Workflow%20(Creating%20a%20new%20listing).png)


### Airtable Workflow – Editing a Listing
![Airtable Workflow – Editing a Listing](screenshots/Airtable%20Workflow%20(Editing%20a%20listing).png)


### Create Listing Page (Bubble Editor
![Create Listing Page (Bubble Editor)](screenshots/Create%20Listing%20Page%20(Bubble%20Editor).png)


### Create Listing Page
![Create Listing Page](screenshots/Create%20Listing%20Page.png)


### Edit Listing Page
![Edit Listing Page](screenshots/Edit%20Listing%20Page.png)


### Header (Bubble Editor
![Header (Bubble Editor)](screenshots/Header%20(Bubble%20Editor).png)


### Login/Signup Page (Bubble Editor
![Login/Signup Page (Bubble Editor)](screenshots/Login_Signup%20Page%20(Bubble%20Editor).png)


### Pricing Page (Bubble Editor
![Pricing Page (Bubble Editor)](screenshots/Pricing%20Page%20(Bubble%20Editor).png)


### Pricing Page
![Pricing Page](screenshots/Pricing%20Page.png)


### Property Listings Page (Bubble Editor
![Property Listings Page (Bubble Editor)](screenshots/Property%20Listings%20Page%20(Bubble%20Editor).png)


### Property Listings Page
![Property Listings Page](screenshots/Property%20Listings%20Page.png)


### Stripe Checkout Session Workflow
![Stripe Checkout Session Workflow](screenshots/Stripe%20Checkout%20Session%20Workflow.png)


### Stripe Workflow – Checkout Session
![Stripe Workflow – Checkout Session](screenshots/Stripe%20Workflow%20(checkout-session).png)


### Stripe Workflow – Invoice Paid
![Stripe Workflow – Invoice Paid](screenshots/Stripe%20Workflow%20(invoice-paid).png)


### Stripe Workflow – Subscription Deleted
![Stripe Workflow – Subscription Deleted](screenshots/Stripe%20Workflow%20(subscription-deleted).png)

---

## Notes
This project is part of a curated **Bubble Developer Portfolio** built for learning purposes.

---

## Creator

**Nachiket Karhade**  
No-Code Builder| Bubble Developer
<br>
🔗 [GitHub](https://github.com/NachiketK43) 
<br>


---
