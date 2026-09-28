<!DOCTYPE html>
<html>
<head>
    <title>1st Quarter Project | Toy Store</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #ffc0cb 0%, #ffc0cb 20%, #ffffff 20%, #ffffff 80%, #87ceeb 80%, #87ceeb 100%);
            min-height: 100vh;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #4a4a4a;
            color: white;
            padding: 15px;
            text-align: center;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
            padding: 5px 12px;
            background-color: #666;
            border-radius: 3px;
            font-size: 14px;
        }
        nav a:hover {
            background-color: #888;
        }
        .main-container {
            display: flex;
            justify-content: space-between;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .left-side, .right-side {
            width: 25%;
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .middle-section {
            width: 45%;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        h2 {
            margin-top: 0;
            padding-bottom: 10px;
            border-bottom: 2px solid #ddd;
        }
        .girls-title {
            color: #ff69b4;
        }
        .boys-title {
            color: #4169e1;
        }
        .toy-item {
            padding: 10px;
            margin: 8px 0;
            background-color: #f9f9f9;
            border: 1px solid #ddd;
            border-radius: 5px;
            cursor: pointer;
        }
        .toy-item:hover {
            background-color: #fffacd;
        }
        .toy-icon {
            font-size: 20px;
            margin-right: 10px;
        }
        .price {
            color: #e74c3c;
            font-weight: bold;
            float: right;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }
        button {
            width: 100%;
            padding: 10px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #45a049;
        }
        .sku-result {
            display: none;
            margin-top: 20px;
            padding: 15px;
            background-color: #e7f3ff;
            border-left: 4px solid #2196F3;
            border-radius: 4px;
        }
        .sku-code {
            font-size: 24px;
            font-weight: bold;
            color: #2196F3;
            letter-spacing: 2px;
            margin: 10px 0;
        }
        .cart {
            margin-top: 20px;
            padding: 15px;
            background-color: #f5f5f5;
            border-radius: 5px;
            max-height: 200px;
            overflow-y: auto;
        }
        .cart-item {
            background: white;
            padding: 8px;
            margin: 5px 0;
            border-radius: 3px;
            display: flex;
            justify-content: space-between;
        }
        .total {
            margin-top: 15px;
            padding: 10px;
            background-color: #4CAF50;
            color: white;
            text-align: center;
            font-size: 18px;
            font-weight: bold;
            border-radius: 4px;
        }
        .receipt-section {
            display: none;
            max-width: 600px;
            margin: 40px auto;
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .receipt-header {
            text-align: center;
            border-bottom: 2px dashed #ccc;
            padding-bottom: 20px;
            margin-bottom: 20px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        th, td {
            padding: 10px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        th {
            background-color: #4CAF50;
            color: white;
        }
        .total-row {
            font-size: 18px;
            font-weight: bold;
            background-color: #4CAF50;
            color: white;
        }
        .receipt-footer {
            text-align: center;
            margin-top: 30px;
            padding-top: 20px;
            border-top: 2px dashed #ccc;
            color: #666;
        }
        .btn {
            display: inline-block;
            margin: 10px 5px;
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            text-decoration: none;
            border-radius: 4px;
            border: none;
            cursor: pointer;
        }
        .btn-print {
            background-color: #2196F3;
        }
        .page-section {
            display: none;
            max-width: 800px;
            margin: 40px auto;
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .page-section h1 {
            color: #333;
        }
        .page-section p {
            line-height: 1.6;
            color: #555;
        }
        .highlight {
            background-color: #fffacd;
            padding: 10px;
            border-left: 4px solid #ffeb3b;
            margin: 20px 0;
        }
        .contact-info {
            text-align: center;
            margin-bottom: 30px;
            color: #666;
        }
    </style>
</head>
<body>
    <header>
        <h1>🧸 TOY STORE</h1>
        <nav>
            <a onclick="showSection('store')">Home & SKU</a>
            <a onclick="showSection('about')">About Us</a>
            <a onclick="showSection('contact')">Contact</a>
        </nav>
    </header>

    <div id="storeSection" class="main-container">
        <div class="left-side">
            <h2 class="girls-title">🌸 Girls Section</h2>
            <div class="toy-item" onclick="addItem('Flower Set', 'GIRLS-FLW', 25, 15.99)">
                <span class="toy-icon">💐</span> Flower Set <span class="price">₱15.99</span>
            </div>
            <div class="toy-item" onclick="addItem('Princess Doll', 'GIRLS-DOL', 30, 24.99)">
                <span class="toy-icon">👸</span> Princess Doll <span class="price">₱24.99</span>
            </div>
            <div class="toy-item" onclick="addItem('Teddy Bear', 'GIRLS-BEA', 40, 19.99)">
                <span class="toy-icon">🧸</span> Teddy Bear <span class="price">19.99</span>
            </div>
            <div class="toy-item" onclick="addItem('Doll House', 'GIRLS-HOU', 15, 49.99)">
                <span class="toy-icon"></span> Doll House <span class="price">₱49.99</span>
            </div>
        </div>

        <div class="middle-section">
            <h2> Order Menu & SKU Generator</h2>
            <div class="form-group">
                <label>Category:</label>
                <select id="category">
                    <option value="GIRLS">Girls Section</option>
                    <option value="BOYS">Boys Section</option>
                </select>
            </div>
            <div class="form-group">
                <label>Product Name:</label>
                <input type="text" id="prodName" placeholder="e.g. Robot Toy">
            </div>
            <div class="form-group">
                <label>Stock Quantity:</label>
                <input type="number" id="stockQty" placeholder="e.g. 50">
            </div>
            <button onclick="generateSKU()">Generate SKU</button>

            <div id="skuDisplay" class="sku-result">
                <strong>Generated SKU:</strong>
                <div id="skuCode" class="sku-code"></div>
                <div id="skuInfo"></div>
            </div>

            <h3 style="margin-top: 30px;">🛒 Current Order:</h3>
            <div id="cart" class="cart">
                <p style="text-align: center; color: #999;">No items yet. Click toys to add!</p>
            </div>
            <div id="totalDiv" class="total" style="display: none;">Total: ₱0.00</div>
            <button onclick="showReceipt()" style="margin-top: 15px; background-color: #ff9800;">Generate Receipt →</button>
        </div>

        <div class="right-side">
            <h2 class="boys-title">🚗 Boys Section</h2>
            <div class="toy-item" onclick="addItem('Race Car', 'BOYS-CAR', 35, 29.99)">
                <span class="toy-icon">🏎️</span> Race Car <span class="price">₱29.99</span>
            </div>
            <div class="toy-item" onclick="addItem('Robot', 'BOYS-ROB', 20, 39.99)">
                <span class="toy-icon">🤖</span> Robot Transformer <span class="price">₱39.99</span>
            </div>
            <div class="toy-item" onclick="addItem('Building Blocks', 'BOYS-BLK', 50, 34.99)">
                <span class="toy-icon">🧱</span> Building Blocks <span class="price">₱34.99</span>
            </div>
            <div class="toy-item" onclick="addItem('RC Car', 'BOYS-RCC', 25, 44.99)">
                <span class="toy-icon">🚙</span> Remote Control Car <span class="price">₱44.99</span>
            </div>
        </div>
    </div>

    <div id="aboutSection" class="page-section">
        <h1>About Our Toy Store</h1>
        <p>Welcome to the best toy store in town! We have been selling toys for kids of all ages since 2020.</p>
        <div class="highlight">
            <h3>Why Choose Us?</h3>
            <ul>
                <li>High quality and safe toys</li>
                <li>Affordable prices in Philippine Peso (₱)</li>
                <li>Separate sections for Boys and Girls</li>
                <li>Fast and friendly service</li>
            </ul>
        </div>
        <h3>Our Mission</h3>
        <p>To bring joy, creativity, and fun to every household.</p>
    </div>

    <div id="contactSection" class="page-section">
        <h1>Contact Us</h1>
        <div class="contact-info">
            <p>📍 123 Main Street, Toy City, Philippines</p>
            <p>📞 (02) 8123-4567</p>
            <p>✉️ info@toystore.ph</p>
        </div>
        <div class="form-group">
            <label>Your Name:</label>
            <input type="text" placeholder="Juan Dela Cruz">
        </div>
        <div class="form-group">
            <label>Email Address:</label>
            <input type="email" placeholder="juan@email.com">
        </div>
        <div class="form-group">
            <label>Message:</label>
            <textarea style="width: 100%; padding: 8px; border: 1px solid #ccc; border-radius: 4px; box-sizing: border-box; font-family: Arial;" rows="5" placeholder="How can we help you?"></textarea>
        </div>
        <button onclick="alert('Thank you! We will get back to you soon.');">Send Message</button>
    </div>

    <div id="receiptSection" class="receipt-section">
        <div class="receipt-header">
            <h2>🧸 TOY STORE 🤖</h2>
            <p>Official Receipt</p>
            <p>123 Main Street, Toy City, Philippines</p>
        </div>
        <div style="margin-bottom: 20px;">
            <p><strong>Receipt #:</strong> <span id="receiptNum"></span></p>
            <p><strong>Date:</strong> <span id="receiptDate"></span></p>
        </div>
        <table>
            <thead>
                <tr>
                    <th>Item</th>
                    <th>SKU</th>
                    <th>Price</th>
                </tr>
            </thead>
            <tbody id="itemsList"></tbody>
            <tfoot>
                <tr class="total-row">
                    <td colspan="2">TOTAL</td>
                    <td id="totalAmt">₱0.00</td>
                </tr>
            </tfoot>
        </table>
        <div class="receipt-footer">
            <p>Thank you for shopping!</p>
            <p>Please come again! 💖</p>
        </div>
        <div style="text-align: center; margin-top: 20px;">
            <button onclick="backToStore()" class="btn">← Back to Store</button>
            <button onclick="window.print()" class="btn btn-print">Print Receipt</button>
        </div>
    </div>

    <script>
        var cart = [];
        var totalAmount = 0;

        function showSection(sectionName) {
            document.getElementById('storeSection').style.display = 'none';
            document.getElementById('aboutSection').style.display = 'none';
            document.getElementById('contactSection').style.display = 'none';
            document.getElementById('receiptSection').style.display = 'none';
            
            if (sectionName == 'store') {
                document.getElementById('storeSection').style.display = 'flex';
            } else if (sectionName == 'about') {
                document.getElementById('aboutSection').style.display = 'block';
            } else if (sectionName == 'contact') {
                document.getElementById('contactSection').style.display = 'block';
            }
            window.scrollTo(0, 0);
        }

        function generateSKU() {
            var category = document.getElementById('category').value;
            var productName = document.getElementById('prodName').value;
            var stockQty = document.getElementById('stockQty').value;
            
            if (productName == '' || stockQty == '') {
                alert('Please fill in all fields!');
                return;
            }
            
            var categoryCode = category.substring(0, 3);
            var productCode = productName.replace(/\s/g, '').substring(0, 3).toUpperCase();
            var sku = categoryCode + '-' + productCode + '-' + stockQty;
            
            document.getElementById('skuCode').innerHTML = sku;
            document.getElementById('skuInfo').innerHTML = 'Category: ' + category + '<br>Product: ' + productName + '<br>Stock: ' + stockQty;
            document.getElementById('skuDisplay').style.display = 'block';
        }

        function addItem(name, code, stock, price) {
            var item = { name: name, code: code, stock: stock, price: price };
            cart.push(item);
            totalAmount += price;
            updateCart();
            var sku = code + '-' + stock;
            alert('Added to cart!\n\nItem: ' + name + '\nSKU: ' + sku + '\nPrice: ₱' + price);
        }

        function updateCart() {
            var cartDiv = document.getElementById('cart');
            var totalDiv = document.getElementById('totalDiv');
            
            if (cart.length == 0) {
                cartDiv.innerHTML = '<p style="text-align: center; color: #999;">No items yet. Click toys to add!</p>';
                totalDiv.style.display = 'none';
                return;
            }
            
            var html = '';
            for (var i = 0; i < cart.length; i++) {
                var item = cart[i];
                html += '<div class="cart-item"><span>' + item.name + '</span><span>₱' + item.price.toFixed(2) + '</span></div>';
            }
            
            cartDiv.innerHTML = html;
            totalDiv.innerHTML = 'Total: ' + totalAmount.toFixed(2);
            totalDiv.style.display = 'block';
        }

        function showReceipt() {
            if (cart.length == 0) {
                alert('Please add items to your cart first!');
                return;
            }
            
            document.getElementById('storeSection').style.display = 'none';
            document.getElementById('receiptSection').style.display = 'block';
            
            var receiptNum = 'RCT-' + Date.now().toString().slice(-8);
            document.getElementById('receiptNum').textContent = receiptNum;
            
            var now = new Date();
            document.getElementById('receiptDate').textContent = now.toLocaleString();
            
            var tbody = document.getElementById('itemsList');
            tbody.innerHTML = '';
            
            for (var i = 0; i < cart.length; i++) {
                var item = cart[i];
                var sku = item.code + '-' + item.stock;
                tbody.innerHTML += '<tr><td>' + item.name + '</td><td>' + sku + '</td><td>₱' + item.price.toFixed(2) + '</td></tr>';
            }
            
            document.getElementById('totalAmt').textContent = '₱' + totalAmount.toFixed(2);
            window.scrollTo(0, 0);
        }

        function backToStore() {
            document.getElementById('receiptSection').style.display = 'none';
            document.getElementById('storeSection').style.display = 'flex';
        }
    </script>
</body>
</html>
