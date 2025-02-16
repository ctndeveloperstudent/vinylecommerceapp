# T3A3-A Assignment: Vinyl eCommerce Platform (MERN)

This repository is the complete documentation for the design and plannning of my MERN stack application: an ecommerce platform built for a vinyl music store. It is built according to the rubric requirements of assignment T3A3-A from Coder Academy.

## R1: Overview (Description of the website including purpose, functionality, target audience and tech stack)

### Description
My website is an eCommerce platform designed specifically for vinyl record enthusiasts, providing a modern, user friendly shopping experience where customers can browse and purchase vinyl records with ease. It features a dark theme, that highlights album covers while ensuring a sleek and intuitive design.

The website's structure is also adaptable for other business owners or artists who want to sell different types of products, making it a versitile eCommerce solution beyond just vinyl records.

### Purpose
This website was created because many vinyl eCommerce platforms lack modern UI/UX, have outdated search features, or provide a poor shopping experience. My goal is to offer a sleek, well-organised marketplace for vinyl lovers while making it easy for independent sellers and artists to list and sell their records.

For business owners looking to sell other types of products, this website can be customised to fit different industries, offering a scalable and user-friendly ecommerce solution.

### Functionality Features
#### For Customers
- Broswe and search vinyl records: customers can explore albums by artist, genre or release year.
- Genre-based filtering: users can filter by pop, rock, alternative, rap, kpop and more.
- Add to cart and check out: Secure checkout with payment options like Stripe or Paypal.
- User accounts: Customers can sign in, login and track their purchases
- Order tracking: Status updates like processing, shipped and delivered to keep the customer informed.
- Responsive design: The plaform is desktop, tablet and mobile phone friendly.

#### For Store Owners/Admin
- Product management: admin can add, edit or delete inventory from the store.
- Order management: admin can update the system and the customer on their order status.
- Stock tracking: The system will keep track of inventory to prevent overselling.
- User management: Admin can manage customer accounts and assign admin roles if needed.

### Target Audience
- Vinyl collectors and enthusiasts: People who prefer physical records over streaming and want an easy way to find rare or classic albums.
- Casual listeners: Those who love music and want to start collecting vinyls.
- Independent artists and sellers: Musicians and small record labels looking for a platform to sell their vinyl releases.
- Small business owners: Entrepreneurs who want to sell non vinyl products by adapting the website to their needs.

### Tech Stack
This project will be built using the MERN stack.
- MongoDB: Stores product data, user accounts and orders.
- Express.js: Backend framework for handling API requests.
- React.js: Frontend for the user interface and interactivity.
- Node.js: Backend runtime environment.
- Stripe/Paypal: For secure payments
- JWT: For secure user and admin authentication  

### Deployment Plan
- Frontend: The website will be deployed on Netlify.
- Backend: The website will be deployed on Render.
- Database: MongoDB Atlas for cloud-based database storage.

## ! R2: Dataflow Diagram
The data flow diagrams were created using the System Structure Analysis and Design Methodology (SSADM) notation system for Dataflow Diagrams.

[Insert diagram here]

## R3 Application Architecture Diagram
The application architecture consists of five main layers, including authentification.

1. User (client side):
    - Users interact with the application through a browser or mobile device.
    - They send HTTP requests to browse records, add items to the cart, and proceed to checkout.

2. Frontend (React - Netlify)
    - The frontend handles UI, routing and API requests.
    - It communicates with the backend using RESTful APIs via Axios.

3. Authentication (JWT - Secure Login)
    - Users log in using JWT authentication, which securely manages sessions.
    - The frontend sends login requests to the backend, which verifies credentials.
    - A JWT token is issued upon successful login and stored on the frontend.
    - The token is included in requests to authenticate user actions (e.g: viewing order history).

4. Backend (Node.js & Express - Render)
    - Processes Api requests coming from the frontend.
    - Manages the business logic, including shopping cart, order processing and authentication.
    - Uses JWT verification to secure user sessions.
    - Contacts to MongoDB Atlas to retrieve or store data.

5. Database (MongoDB - Cloud Based Storage)
    - Stores user accounts, products, orders, payments, and inventory.
    - Ensures data persistence and security.

### Diagram
[Insert Application Architecture Diagram Here]

## R4: User Stories & Personas (Progress and Refinement)

### First Iteration of User Stories

User Story 1: Browsing & Filtering Records

- "As a vinyl collector, I want to browse and filter records by genre, artist, and release year, so that I can quickly find albums that match my collection interests."

User Story 2: Secure Login & Order Tracking

- "As a casual music listener, I want to create an account and securely log in, so that I can track my orders and manage my purchases."

User Story 3: Product Management for Sellers

- "As an independent vinyl seller, I want to list my records for sale and update stock availability, so that I can manage my inventory efficiently and keep customers informed."

User Story 4: Order Status Updates

- "As an online shopper, I want to receive order status updates (Processing, Shipped, Delivered), so that I know when to expect my order."

### First Iteration of Personas

#### Persona 1: Aria (Vinyl Collector)

Background: A dedicated vinyl collector who enjoys rare and classic records.

Goals:
- Find specific vinyl records quickly.
- Complete collections and discover new releases.

Pain Points:
- Struggles with eCommerce sites that lack filtering options.
- Finds it frustrating when album details (artist, release year) are missing.

#### Persona 2: Spencer (Casual Listener)

Background: A casual music fan who is just starting to collect vinyls.

Goals:
- Buy a few favorite records.
- Easily track purchases and past orders.

Pain Points:
- Worried about account security when shopping online.
- Finds order tracking difficult on some platforms.

#### Persona 3: Alison (Independent Vinyl Seller)

Background: A small business owner who sells limited-edition, newly released and second-hand vinyl.

Goals:
- List vinyl records for sale easily.
- Update stock availability to prevent overselling.

Pain Points:
- Manual inventory management is time-consuming.
- Large platforms take high commission fees.


#### Persona 4: Hanna (Online Shopper)

Background: A frequent online buyer who loves convenience and clear tracking information.

Goals:
- Receive real-time order updates.
- Know exactly when their purchase will arrive.

Pain Points:
- Frustrated by unclear delivery times.
- Has had issues with orders getting lost due to lack of updates.


### Updates & Refinements 

- Aria’s user story aligns with enhanced search and filtering features → Updated to include artist and release year search.

- Spencer’s user story emphasizes JWT authentication for secure logins → Updated to include forgotten password recovery.

- Alison’s user story focuses on inventory and stock management → Updated to include bulk product uploading for efficiency.

- Hanna’s user story highlights the importance of order tracking updates → Updated to include email notifications for tracking updates.


### Finalized & Updated Personas

#### Aria – The Vinyl Collector

Background: A dedicated vinyl collector who enjoys rare and classic records.

Goals:
- Find specific vinyl records quickly.
- Complete collections and discover new releases.
- Use artist and release year search to refine results.

Pain Points:
- Struggles with eCommerce sites that lack filtering options.
- Finds it frustrating when album details (artist, release year) are missing.

How My Website Helps:
- Genre-based filtering makes it easier to find records.
- Search by artist and release year for precise results.
- Clear album descriptions help users make informed purchases.


#### Spencer – The Casual Listener

Background: A casual music fan who is just starting to collect vinyl.

Goals:
- Buy a few favorite records.
- Easily track purchases and past orders.
- Ensure secure transactions and password recovery options.

Pain Points:
- Worried about account security when shopping online.
- Finds order tracking difficult on some platforms.

How My Website Helps:
- JWT authentication ensures secure login and session management.
- User dashboard shows past purchases and current orders.
- Forgot password recovery for account security.


#### Alison – The Independent Vinyl Seller

Background: A small business owner who sells limited-edition and second-hand vinyl.

Goals:
- List vinyl records for sale easily.
- Update stock availability to prevent overselling.
- Bulk upload product listings for efficiency.

Pain Points:
- Manual inventory management is time-consuming.
- Large platforms take high commission fees.

How My Website Helps:
- Simple product management for adding, editing, and removing records.
- Stock tracking prevents overselling.
- Bulk upload feature for faster inventory updates.


#### Hanna – The Online Shopper

Background: A frequent online buyer who loves convenience and clear tracking information.

Goals:
- Receive real-time order updates.
- Know exactly when their purchase will arrive.
- Get email notifications for delivery updates.

Pain Points:
- Frustrated by unclear delivery times.
- Has had issues with orders getting lost due to lack of updates.

How My Website Helps:
- Order status tracking (Processing, Shipped, Delivered).
- Email notifications keep customers informed.
- Clear shipping policies with estimated delivery times.


### Updated User Stories Based on Persona Revisions

Updated User Story 1: Browsing & Filtering Records

- "As a vinyl collector, I want to browse and filter records by genre, artist, and release year, so that I can quickly find albums that match my collection interests and refine my search results."

Updated User Story 2: Secure Login & Password Recovery

- "As a casual music listener, I want to create an account, securely log in using JWT authentication, and recover my password if needed, so that I can access my orders without security concerns."

Updated User Story 3: Bulk Product Management for Sellers

- "As an independent vinyl seller, I want to list my records for sale, update stock availability, and bulk upload products, so that I can manage my inventory efficiently and keep customers informed."

Updated User Story 4: Order Status Updates with Email Notifications

- "As an online shopper, I want to receive order status updates via email (Processing, Shipped, Delivered), so that I know when to expect my vinyl purchase and avoid missed deliveries."


### Summary of Progress & Refinement

- Created initial user stories based on core website features.
- Developed personas to align with key user groups.
- Updated personas based on user story needs (added filtering, password recovery, bulk upload, and email notifications).
- Refined user stories to include these updates for a more detailed, trackable feature roadmap.