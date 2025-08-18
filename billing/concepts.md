In this blog we will outline some of the key concepts that is needed for understanding the Killbill. as a platform

##### Background Concepts

- **Customer** – someone who buys your product
- **Administrator** (or **Admin**) – the person who can use the Kill Bill UI to view and modify customer accounts
- **Kill Bill Administrator** (or **Kill Bill Admin**) - the person responsible for installing or configuring Kill Bill
- **Account** – a customer account. It represents what Kill Bill knows about a customer.
- **Subscription** – a contract between you and a customer to purchase a particular product with particular terms. In the system it associates a Plan (see below) with an Account and a start date.
- **Subscription Bundle** (or just **Bundle**) – a collection of subscriptions that are associated with a particular instance of a product. For example, you might have a voice plan, a data plan and a text plan for your mobile phone. In Kill Bill each plan would have its own subscription and we would represent the fact that they are associated with a single phone by grouping them in a Subscription Bundle. Of course an account might have multiple phones associated with it and a Kill Bill Account can have multiple Bundles associated with it.
## Catalog
The Catalog is a data model that captures the core configuration of the billing system. This model is at the heart of the billing system. It is very important that all the business logic associated with the billing behaviour of your system is captured in the billing system.

A Kill Bill Catalog includes the following sections:

- **Products**




### Rules

Types of Rules that is present in the KillBill.

- Billing alignment rules
- Subscription alignment rules
	- Add on phase alignment
	- Plan cancellation timing: Available options:
		- END_OF_TERM
		- IMMEDIATE
	- Plan change timing: Available options:
		- END_OF_TERM
		- IMMEDIATE
		- ILLEGAL
	- 
	- 