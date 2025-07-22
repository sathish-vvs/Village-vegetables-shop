<!DOCTYPE html>
<html>
  <head>
    <title>VVS Shop</title>
  </head>
  <body>
    <h1>Village Vegetable Shop</h1>
    <input id="itemName" placeholder="Enter item name" />
    <input id="itemPrice" placeholder="Enter price" type="number" />
    <button onclick="addItem()">Add Item</button>

    <ul id="itemList"></ul>

    <script>
      function addItem() {
        const name = document.getElementById('itemName').value;
        const price = document.getElementById('itemPrice').value;
        const li = document.createElement('li');
        li.innerText = `${name} - ₹${price}`;
        document.getElementById('itemList').appendChild(li);
      }
    </script>
  </body>
</html>
