# TASK 5

* Create atleast 10 records using the save method

```ruby =

id: 1,
 name: "Cowhead",
 description: "Pure Milk Drink",
 quantity: 2,
 price: 109.5,
 available: true,
 released_at: Tue, 01 Oct 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 2,
 created_at: Tue, 01 Oct 2024 15:25:35.784535000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:25:35.784535000 UTC +00:00>

id: 2,
 name: "Arla Milk Goodness",
 description: "Low Fat Milk Drink",
 quantity: 1,
 price: 121.5,
 available: true,
 released_at: Mon, 23 Jan 2023 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 1,
 created_at: Tue, 01 Oct 2024 15:34:37.845453000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:34:37.845453000 UTC +00:00>

 id: 3,
 name: "Bear Brand Choco Drink",
 description: "Fortified Milk Drink",
 quantity: 3,
 price: 240.0,
 available: true,
 released_at: Sat, 01 Jan 2022 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 0,
 created_at: Tue, 01 Oct 2024 15:37:32.599797000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:37:32.599797000 UTC +00:00>

 id: 4,
 name: "Selecta Milk Drink",
 description: "Fortified Milk Drink",
 quantity: 1,
 price: 70.0,
 available: true,
 released_at: Sun, 25 Feb 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 1,
 created_at: Tue, 01 Oct 2024 15:39:39.613871000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:39:39.613871000 UTC +00:00>

 id: 5,
 name: "So Good Oat Drink",
 description: "Oats Drink",
 quantity: 1,
 price: 50.0,
 available: false,
 released_at: Sat, 25 May 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 0,
 created_at: Tue, 01 Oct 2024 15:42:08.107815000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:42:08.107815000 UTC +00:00>

 id: 6,
 name: "Kirkland Signature Drink",
 description: "Soymilk",
 quantity: 1,
 price: 85.0,
 available: true,
 released_at: Fri, 22 Mar 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 0,
 created_at: Tue, 01 Oct 2024 15:44:23.812314000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:44:23.812314000 UTC +00:00>

 id: 7,
 name: "Birch Tree",
 description: "Fortified Milk Drink",
 quantity: 3,
 price: 120.0,
 available: true,
 released_at: Fri, 22 Mar 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 10,
 created_at: Tue, 01 Oct 2024 15:46:20.996397000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:46:20.996397000 UTC +00:00>

 id: 8,
 name: "Nestle Non-Fat Calcium Drink",
 description: "Non-Fat Drink",
 quantity: 1,
 price: 48.0,
 available: true,
 released_at: Fri, 22 Mar 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 10,
 created_at: Tue, 01 Oct 2024 15:49:54.410084000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:49:54.410084000 UTC +00:00>

 id: 9,
 name: "Hacienda Macalauan Milk Drink",
 description: "Fresh Whole Milk Drink",
 quantity: 1,
 price: 165.0,
 available: true,
 released_at: Tue, 22 Oct 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 2,
 created_at: Tue, 01 Oct 2024 15:51:53.223207000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:51:53.223207000 UTC +00:00>

 id: 10,
 name: "Emborg Full Milk",
 description: "Fresh Whole Milk Drink",
 quantity: 2,
 price: 98.0,
 available: true,
 released_at: Mon, 24 Jun 2024 00:00:00.000000000 UTC +00:00,
 expiry_date: nil,
 discount: 1,
 created_at: Tue, 01 Oct 2024 15:55:42.125436000 UTC +00:00,
 updated_at: Tue, 01 Oct 2024 15:55:42.125436000 UTC +00:00>
```
* Create atleast 10 records using the save method

```ruby =
product = Products.new
product.name = 'Cheddar Cheese'
product.description = 'Natural Cheese'
product.quantity = 1
product.price = 65.00
product.available = true
product.released_at = DateTime.now - 5
product.expiry_date = DateTime.now + 6
product.discount = 1.00
product.save

product = Products.new
product.name = 'Gouda Cheese'
product.description = "Creamy Yellow from Cow's Milk"
product.quantity = 2
product.price = 265.00
product.available = true
product.released_at = DateTime.now - 4
product.expiry_date = DateTime.now + 8
product.discount = 3.00
product.save

product = Products.new
product.name = 'Goat Cheese'
product.description = "Fresh Soft from Goat's Milk"
product.quantity = 2
product.price = 150.00
product.available = true
product.released_at = DateTime.now - 2
product.expiry_date = DateTime.now + 45
product.discount = 15.00
product.save

product = Products.new
product.name = 'Cream Cheese'
product.description = 'Soft Mild Tasting Cheese'
product.quantity = 1
product.price = 75.00
product.available = false
product.released_at = DateTime.now - 1
product.expiry_date = DateTime.now + 35
product.discount = 2.00
product.save

product = Products.new
product.name = 'Mozzarella Cheese'
product.description = 'Semi Soft Non-Aged Cheese'
product.quantity = 2
product.price = 500.00
product.available = true
product.released_at = DateTime.now - 1
product.expiry_date = DateTime.now + 65
product.discount = 12.00
product.save

product = Products.new
product.name = 'Hard Cheese'
product.description = 'Extra Hard Cheese'
product.quantity = 1
product.price = 2050.00
product.available = false
product.released_at = DateTime.now - 4
product.expiry_date = DateTime.now + 150
product.discount = 25.00
product.save

product = Products.new
product.name = 'Blue Cheese'
product.description = 'made from cultured edible molds'
product.quantity = 3
product.price = 650.00
product.available = true
product.released_at = DateTime.now - 1
product.expiry_date = DateTime.now + 75
product.discount = 5.00
product.save

product = Products.new
product.name = 'Feta Cheese'
product.description = "Made from Sheep's Milk"
product.quantity = 2
product.price = 180.00
product.available = true
product.released_at = DateTime.now - 6
product.expiry_date = DateTime.now + 95
product.discount = 12.00
product.save

product = Products.new
product.name = 'Brie Cheese'
product.description = 'pale coloured greyish cheese'
product.quantity = 1
product.price = 120.00
product.available = false
product.released_at = DateTime.now - 2
product.expiry_date = DateTime.now + 6
product.discount = 1.00
product.save

product = Products.new
product.name = 'Cottage Cheese'
product.description = 'curdled milk product'
product.quantity = 1
product.price = 350.00
product.available = true
product.released_at = DateTime.now - 5
product.expiry_date = DateTime.now + 45
product.discount = 3.00
product.save
```

* Fetch all products where name is "Laptop".
```ruby =
  Products.where(name: 'Laptop')
```

* Find products where price is greater than 100.
```ruby =
Products.where('price > ?', 100)
```

* Retrieve products where available is true.
```ruby = 
Products.where(available: true) 
```

* Fetch products where quantity is less than 50.
```ruby =
Products.where('quantity < ?', 50)
```

* Find products where discount is exactly 10%.
```ruby =
Products.where('discount =?', 10)
```
* Retrieve products where name contains the word Pro.
```ruby =
Products.where('name LIKE ?', '%Pro%')
```
* Fetch products where description includes the word "portable".
```ruby =
Products.where(description: 'portable')
```