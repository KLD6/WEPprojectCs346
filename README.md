<html>
<body>
<!--StartFragment--><html><head></head><body><h1>Product Management System (PMS)</h1>
<h2>Introduction</h2>
<p><strong>Product Management System (PMS)</strong> is a <strong>CRUD-based application</strong> built using <strong>Node.js, Express, MongoDB, and JavaScript</strong>. It allows users to <strong>Create, Read, Update, and Delete</strong> product records with real-time UI updates and search functionality.</p>
<h3> <strong>Key Features</strong></h3>
<ul>
<li><strong>Product Management</strong> – Add, edit, and delete products.</li>
<li><strong>Real-time UI updates</strong> – Changes reflect instantly.</li>
<li><strong>Search Functionality</strong> – Filter by title or category.</li>
<li><strong>Database-Driven</strong> – Uses MongoDB instead of Local Storage.</li>
<li><strong>RESTful API</strong> – Backend for handling CRUD operations.</li>
</ul>
<hr>
<h2> Installation Guide</h2>
<h3><strong>Prerequisites</strong></h3>
<ul>
<li><strong>Node.js</strong> (Latest LTS version)</li>
<li><strong>MongoDB</strong> (Local or Atlas Cloud)</li>
</ul>
<h3> <strong>Installation Steps</strong></h3>

# Install dependencies
npm install

# Start MongoDB server (if running locally)
mongod

# Run the backend
npm start
</code></pre>
<p>Your server should now be running at: <code inline="">http://localhost:5000</code></p>
<hr>
<h2> Usage Guide</h2>
<h3> <strong>Running the Application</strong></h3>
<p>1 <strong>Start the backend:</strong> <code inline="">npm start</code><br>
2 <strong>Open <code inline="">http://localhost:5000</code> in the browser</strong><br>
3 <strong>Perform CRUD operations:</strong></p>
<ul>
<li><strong>Create a product</strong> – Fill the form &amp; click <strong>Create</strong>.</li>
<li><strong>View products</strong> – Products appear in the table.</li>
<li><strong>Update a product</strong> – Click <strong>Update</strong>, modify details, and save.</li>
<li><strong>Delete a product</strong> – Click <strong>Delete</strong> next to any product.</li>
<li><strong>Search</strong> – Use <strong>Search by Title</strong> or <strong>Search by Category</strong>.</li>
</ul>
<hr>
<h2> API Documentation</h2>
<h3><strong> Base URL:</strong></h3>
<pre><code>http://localhost:5000
</code></pre>
<h3><strong> Available Endpoints:</strong></h3>

Method | Endpoint | Description
-- | -- | --
GET | /api/products | Fetch all products
POST | /api/products | Add a new product
PUT | /api/products/:id | Update a product
DELETE | /api/products/:id | Delete a product


<h4><strong>Example: Adding a Product</strong></h4>
<pre><code class="language-sh">curl -X POST "http://localhost:5000/api/products" -H "Content-Type: application/json" -d '{
  "title": "Phone",
  "price": 100,
  "ads": 5,
  "taxes": 10,
  "discount": 2,
  "total": 113,
  "count": 1,
  "category": "Electronics"
}'
</code></pre>
<hr>
<h2>🛑 Challenges &amp; Solutions</h2>
<h3><strong>1- Transition from Local Storage to MongoDB</strong></h3>
<ul>
<li><strong>Problem:</strong> UI updates worked instantly in Local Storage but broke with MongoDB.</li>
<li><strong>Solution:</strong> Used <code inline="">fetchProducts()</code> to re-fetch products after every CRUD action.</li>
</ul>
<h3><strong>2- Fixing Search Issues</strong></h3>
<ul>
<li><strong>Problem:</strong> <code inline="">GetSearchMood is not defined</code> error.</li>
<li><strong>Solution:</strong> Re-added <code inline="">GetSearchMood()</code> function and connected search buttons correctly.</li>
</ul>
<h3><strong>3- Ensuring Data Consistency</strong></h3>
<ul>
<li><strong>Problem:</strong> Duplicate product entries due to <code inline="">count</code> field.</li>
<li><strong>Solution:</strong> Looped product creation logic only when necessary.</li>
</ul>

<hr>
<h3> <strong>Contributors</strong></h3>
<ul>
<li><strong>Project Lead:</strong> [KHALID WALEED ALSUNAYDIH-443016780]</li>
<li><strong>Developer:</strong> [BADER FAHAD ALMASOUD-443017986]</li>
<li><strong>Developer:</strong> [KHALID NAFEA HOSAH-443016589]</li>
<li><strong>Developer:</strong> [ABDULLAH HAMDAN ALDOSARI-444002393]</li>
</ul>
</body>
</html>
