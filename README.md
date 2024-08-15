<h1>ShopRush Web Application Documentation</h1>
<h4>URL of the project -> https://shoprush.onrender.com</h4>
<h4>NOTE: When you open the URL, sometimes you will wait 10-20 seconds to start the app, because of the free domain which i used!</h4>

<h3>Welcome to the official documentation for ShopRush, a dynamic web application built using the Express framework and powered by MongoDB for efficient database management. ShopRush offers a comprehensive online shopping experience, enabling users to seamlessly perform actions like user registration, login, logout, product creation, and more.</h3>

 <h2>Table of Contents</h2>
    <ol>
        <li><a href="#introduction">Introduction</a></li>
        <li>
            <a href="#getting-started">Getting Started</a>
            <ul>
                <li><a href="#installation">Installation</a></li>
                <li><a href="#configuration">Configuration</a></li>
            </ul>
        </li>
        <li>
            <a href="#usage">Usage</a>
            <ul>
                <li><a href="#user-authentication">User Authentication</a></li>
                <li><a href="#product-management">Product Management</a></li>
            </ul>
        </li>
        <li><a href="#api-reference">API Reference</a></li>
        <li>
            <a href="#database">Database</a>
        </li>
        <li><a href="#contributing">Contributing</a></li>
        <li><a href="#license">License</a></li>
    </ol>
    <h2 id="introduction">Introduction</h2>
    <p>Welcome to <strong>ShopRush</strong>! This documentation provides a comprehensive guide to the features and functionality of our web application. ShopRush is built on the Express framework and leverages MongoDB as its backend database. It replicates the shopping experience, allowing users to explore products, manage their accounts, and interact with an intuitive interface.</p>

<h2 id="getting-started">Getting Started</h2>

  <h3 id="installation">Installation</h3>

  <p>1. <strong>Clone the Repository:</strong></p>
  <pre><code>git clone https://github.com/Bogomil-Simitchiev/ShopRush</code></pre>

  <p>2. <strong>Navigate to the Project Directory:</strong></p>
  <pre><code>cd ShopRush</code></pre>

  <p>3. <strong>Install Dependencies:</strong></p>
  <pre><code>npm install</code></pre>

   <p>4. <strong>Start the Application:</strong></p>
  <pre><code>npm start</code></pre>
  
  <h3 id="configuration">Configuration</h3>

  <p>Configure the application by setting up environment variables in files located in the project folders. Required variables include:</p>

   <ul>
        <li><code>MONGODB_NAME</code>: MongoDB username.</li>
        <li><code>MONGODB_PASSWORD</code>: MongoDB username.</li>
        <li><code>MONGODB_DBNAME</code>: MongoDB database name (I used "shop")</li>
        <li><code>SENDGRID_KEY</code>: SendGrid api key.</li>
        <li><code>STRIPESECRET_KEY</code>: Stripe secret api key.</li>

  </ul>

   <h2 id="usage">Usage</h2>

   <h3 id="user-authentication">User Authentication</h3>

   <p>ShopRush offers robust user authentication functionalities:</p>

  <ul>
        <li><strong>Signup:</strong> New users can create accounts by providing their email and password.</li>
        <li><strong>Login:</strong> Registered users can securely log in with their credentials.</li>
        <li><strong>Logout:</strong> Logged-in users can easily log out of their accounts.</li>
  </ul>

   <h3 id="product-management">Product Management</h3>

  <p>ShopRush simplifies product management:</p>

  <ul>
        <li><strong>Create Product:</strong> Authenticated users can effortlessly add new products, including details like name, description, price, and images.</li>
        <li><strong>View Products:</strong> Customers can explore the diverse product range.</li>
        <li><strong>Update Product:</strong> Admin users possess the privilege to edit product information.</li>
        <li><strong>Delete Product:</strong> Admin users can seamlessly remove products from the catalog.</li>
    </ul>
    <h2 id="api-reference">API Reference</h2>

  <h3 id="authentication-endpoints">Authentication Endpoints</h3>
    <ul>
        <li><code>POST /signup</code>: Create a new user account.</li>
        <li><code>POST /login</code>: Log in as an existing user.</li>
        <li><code>POST /logout</code>: Log out from the current session.</li>
    </ul>
 <h3 id="product-endpoints">Product Endpoints</h3>
    <ul>
        <li><code>POST /admin/add-product</code>: Create a new product (Admin access required).</li>
        <li><code>GET /products</code>: Retrieve a list of all products.</li>
        <li><code>GET /products/:id</code>: Retrieve details of a specific product.</li>
        <li><code>PUT /admin/edit-product/:id</code>: Update product details (Admin access required).</li>
        <li><code>DELETE /products/:id</code>: Delete a product (Admin access required).</li>
    </ul>
     <h2 id="database">Database</h2>

  <p>ShopRush employs MongoDB to efficiently manage user data, product information, order data and session details. The application interacts with the database using the Mongoose library.</p>

  <h2 id="contributing">Contributing</h2>

  <p>We heartily welcome contributions to enhance ShopRush! If you encounter any issues or have innovative ideas, kindly open an issue or submit a pull request on my GitHub repository.</p>

  <h2 id="license">License</h2>

  <p>ShopRush operates under the <a href="https://opensource.org/licenses/MIT">MIT License</a>.</p>
