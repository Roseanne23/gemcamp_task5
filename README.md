# TASK 5

* Create atleast 10 records using the create method

```ruby =
Products.create(name: 'Cowhead', description: 'Pure Milk Drink', quantity: 2, price: 109.50, available: true, released_at: Date.new(2024, 10, 1), expiry_date: nil, discount: 2.0)
Products.create(name: 'Arla Milk Goodness', description: 'Low Fat Milk Drink', quantity: 1, price: 121.50, available: true, released_at: Date.new(2023, 01, 23), expiry_date: nil, discount: 1.0)
Products.create(name: 'Bear Brand Choco Drink', description: 'Fortified Milk Drink', quantity: 3, price: 240.00, available: true, released_at: Date.new(2022, 01, 01), expiry_date: nil, discount: 0.50)
Products.create(name: 'Selecta Milk Drink', description: 'Fortified Milk Drink', quantity: 1, price: 70.00, available: true, released_at: Date.new(2024, 02, 25), expiry_date: nil, discount: 1.50)
Products.create(name: 'So Good Oat Drink', description: 'Oats Drink', quantity: 1, price: 50.00, available: false, released_at: Date.new(2024, 05, 25), expiry_date: nil, discount: 0.70)
Products.create(name: 'Kirkland Signature Drink', description: 'Soymilk', quantity: 1, price: 85.00, available: true, released_at: Date.new(2024, 03, 22), expiry_date: Date.today, discount: 0.50)
Products.create(name: 'Nestle Non-Fat Calcium Drink', description: 'Non-Fat Drink', quantity: 1, price: 48.00, available: true, released_at: Date.new(2024, 03, 22), expiry_date: nil, discount: 10.00)
Products.create(name: 'Hacienda Macalauan Milk Drink', description: 'Fresh Whole Milk Drink', quantity: 10, price: 1650.00, available: true, released_at: Date.new(2024, 10, 22), expiry_date: nil, discount: 2.00)
Products.create(name: 'Emborg Full Milk', description: 'Fresh Whole Milk Drink', quantity: 2, price: 98.00, available: true, released_at: Date.new(2024, 06, 24), expiry_date: nil, discount: 1.00)
Products.create(name: 'Binggrae Banana Milk Pro', description: 'Out of stock', quantity: 50, price: 45.00, available: true, released_at: Date.new(2021, 12, 24), expiry_date: Date.today, discount: 15.00)
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

* Find products where price is between 50 and 150.
```ruby =
Products.where(price: 50..150)
```

* Retrieve products where available is false and quantity is greater than 0.
```ruby =
Products.where(available: false).where('quantity > ?', 0)
```

* Fetch products where released_at is after January 1, 2023.
```ruby =
Products.where('released_at > ?', Date.new(2023, 1, 1))
```

* Find products where expiry_date is nil.
```ruby =
Products.where(expiry_date: nil)
```

* Retrieve products where released_at is before January 1, 2022.
```ruby =
Products.where('released_at > ?', Date.new(2022, 1, 1))
```

* Fetch products where quantity is between 10 and 100.
```ruby =
Products.where(quantity: 10..100)
```

* Find products where discount is greater than or equal to 5%.
```ruby =
Products.where('discount >= ?',5)
```
* Retrieve products where price is less than or equal to 200 and available is true
```ruby =
Products.where('price <= ? && available = ?', 200, true)
```

* Fetch products where expiry_date is before today’s date
```ruby =
Products.where('expiry_date < ?', Date.today)
```

* Find products where name starts with the letter "A"
```ruby =
Products.where("name LIKE ?", "A%")
```

* Retrieve products where price is not equal to 100
```ruby =
Products.where.not(price: 100)
```

* Fetch products where quantity is nil
```ruby =
Products.where(quantity: nil)
```

* Find products where discount is not nil
```ruby =
Products.where.not(discount: nil)
```

* Update the price of a product where name is "Laptop" to 120
```ruby =
Products.where(name: "Laptop").update_all(price: 120)
```

* Set the available status to false for products where quantity is 0
```ruby =
Products.where(quantity: 0).update_all(available: false)
```

* Increase the discount by 5% for products where price is greater than 100
```ruby =
Products.where("price > ?", 100).update_all("discount = discount * 1.05")
```

* Update the description to "Out of stock" for products where available is false
```ruby = 
Products.where(available: false).update_all(description: "Out of stock")
```

* Change the expiry_date to December 31, 2024, for products with a discount greater than 10%
```ruby = 
Products.where("discount > ?", 10).update_all(expiry_date: "2024-12-31")
``` 

* Update the quantity to 50 for products where name starts with "Pro"
```ruby = 
Products.where("name LIKE ?", "Pro%").update_all(quantity: 50)
``` 

* Set the price to 200 for all products where discount is nil
```ruby = 
Products.where(discount: nil).update_all(price: 200)
``` 

* Mark products as available if their released_at is before January 1, 2023
```ruby = 
Products.where("released_at < ?", Date.new(2023, 1, 1)).update_all(available: true)
``` 

* Update the price to 80 where the quantity is between 10 and 20
```ruby = 
Products.where(quantity: 10..20).update_all(price: 80)
``` 