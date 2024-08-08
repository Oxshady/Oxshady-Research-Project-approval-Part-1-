# EgyXpress

## Table of Contents:
1. [Team Members](#team-members)
2. [Technologies](#technologies)
3. [Challenge](#challenge)
4. [Risks](#risks)
5. [Infrastructure](#infrastructure)
6. [Existing Solutions](#existing-solutions)

## Team Members:
1. **Shadi Mahmoud**  
   - **Role:** Backend Developer  
   - **Responsibilities:** Designing and implementing the custom API and managing server-side logic. This role focuses on building core functionality and integrating with third-party APIs.

2. **Ahmed Khaled**  
   - **Role:** Backend Developer  
   - **Responsibilities:** Handles deployment, automation, and server management tasks. This role ensures the application is efficiently deployed, secure, and optimized for performance.

3. **Sondos Essam**  
   - **Role:** Frontend Developer  
   - **Responsibilities:** Develops the user interface and ensures a seamless integration with the back-end API. This role is focused on creating an intuitive and responsive user experience.

## Technologies

### Backend Framework:
We will use Flask for our web framework because it’s simple, efficient, and easy to extend with various services. Python will be used to handle business logic and create models.

**Other options:** (Node.js, Express.js, Django)  
Flask was preferred because it is sufficient for the project at hand, and the extra features and functionalities that other frameworks provide won’t be mostly used.

### Database Management System:
Relational databases will be used with a master-slave configuration to handle write operations on the master database and distribute the read operations on both the master and slave databases to improve user experience and reduce reading time. We will use ORM (Object Relational Mapping) to map classes to tables so everything will be object-oriented.

**Other option:** (NoSQL)  
Relational databases were chosen due to the need for structured data, which NoSQL cannot provide.

### Frontend Technologies:
We will use HTML, CSS, and Bootstrap to build and style web pages. JavaScript will add interactive features, with React enhancing user interface development and state management, and jQuery will help fetch data from different endpoints without refreshing the page.

**Other options:** (Vue.js)  
Unlike Vue.js, React is known for its flexibility and can be easily integrated with other libraries and frameworks. It allows for a modular approach, where developers can pick and choose different tools that fit their needs.

### APIs:
We will build a REST API that supports all CRUD operations and follows most REST constraints.

**Other option:** (GraphQL)  
REST was chosen because it’s simpler and more widely adopted for many use cases.

## Challenge

Our eCommerce platform addresses key challenges faced by Egyptian consumers, including the difficulty of purchasing international goods due to strict regulations on paying in USD and the lack of localized online shopping options. By offering a wide range of products, from electronics to household goods, and providing features like local payment methods, fast delivery, and customer support in Arabic, the platform aims to deliver a comprehensive shopping experience tailored to the Egyptian market.

Targeting a broad audience, including young professionals, students, families, and small business owners, the platform combines localized digital marketing strategies, such as social media campaigns and influencer collaborations, with traditional methods like billboards and radio ads. Additionally, launch promotions, referral programs, and community engagement will build trust and drive user engagement, ensuring the platform effectively meets local needs while establishing a strong brand presence in Egypt.

## Risks

### Technical Risks:
1. **Security Risks:**  
   **Risk:** Our e-commerce site could be vulnerable to attacks like data breaches or SQL injection, which might expose customer and financial information.  
   **Solution:** Implement SSL/TLS encryption for secure data transmission, use secure coding practices, and set up regular security checks to find and fix vulnerabilities.

2. **Performance Issues:**  
   **Risk:** Slow site loading or server overloads might hurt user experience and sales.  
   **Solution:** Implement caching to speed up the site and use a load balancer to manage traffic and cache static content.

3. **Data Loss:**  
   **Risk:** Data could be accidentally deleted or corrupted, disrupting operations and affecting customer data.  
   **Solution:** Set up a backup system to regularly save data and create a disaster recovery plan to quickly restore data if something goes wrong.

### Non-Technical Risks:
1. **Budget Constraints:**  
   **Risk:** Limited money for marketing.  
   **Solution:** Use inexpensive methods like SEO and free social media ads.

2. **Customer Retention:**  
   **Risk:** It might be hard to attract and keep customers.  
   **Solution:** Set up a rewards program and improve based on customer feedback.

3. **Customer Service Challenges:**  
   **Solution:** Listen to customer feedback to fix problems and improve services.

## Infrastructure

### Branching and Merging:
- Employ the GitHub Flow strategy.
- Develop each feature or bug fix in a separate branch.
- Merge completed and reviewed feature branches into the main branch through pull requests to ensure code stability and thorough testing.

### Deployment Strategy:
- Manage deployment and automation using the Fabric extension.
- Utilize Nginx as the web server and Flask as the application server.
- Initially deploy the application to a staging environment for testing, and upon successful validation, proceed with deployment to the production environment.

### Infrastructure Details:
- **Nginx Web Servers:** Use two Nginx servers to handle HTTP requests efficiently.
- **HAProxy Load Balancer:** Deploy HAProxy as the load balancer to distribute traffic and manage SSL/TLS termination, enhancing security and performance.
- **MySQL Configuration:** Implement a master-slave MySQL setup to balance read and write operations, improving database performance and redundancy.

### Data Population:
- Develop a custom API to manage data interactions.
- Start with dummy data to simulate real-world conditions.
- Populate the application with real-time data from partner suppliers and third-party APIs as the project progresses.

### Testing Tools and Processes:
- Adopt the Test-Driven Development (TDD) approach, ensuring that tests are written before the code.

## Existing Solutions

The proposed e-commerce project shares similarities with major platforms like Amazon, eBay, and Walmart but also introduces unique features. Like Amazon, our platform will offer a wide range of product categories and a marketplace for third-party sellers, but with a stronger emphasis on personalized user experiences and targeting niche markets. While eBay allows third-party sellers and offers a variety of goods, our platform will focus on fixed-price sales, avoiding the auction model, and incorporate advanced features like augmented reality (AR) for product visualization. Similar to Walmart, our platform will offer a broad range of products, but will prioritize quality and exclusivity in its offerings. Additionally, we will enhance the user experience with a superior user interface and online shopping experience, distinguishing our platform from these existing solutions.
