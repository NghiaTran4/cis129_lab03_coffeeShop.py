# cis129_lab03_coffeeShop.py
print("My Coffee and Muffin Shop")

print("Menu of My Coffee and Muffin Shop")
print("1 Coffee at $5 each")
print("1 Muffins at $4 each")
print("1 Donus at $3 each")
print("1 Cookie at $2 each")
print("6% tax")

def calculate_total(coffe, muffin, donus, cookie):
  # calculate 
  coffe_price = 5
  muffin_price = 4
  donus_price = 3
  cookie_price = 2
  subtotal = (coffe * coffe_price) + (muffin * muffin_price) + (donus * donus_price) + (cookie * cookie_price)

  # Tax
  tax_price = 0.06
  tax = subtotal * tax_price

  # Total
  total = subtotal + tax

  return total

def main():
  # Number of item 
  coffe = int(input("Enter number of coffe: "))
  muffin = int(input("Enter number of muffin: "))
  donus = int(input("Enter number of donus: "))
  cookie = int(input("Enter number of cookie: "))

  # calculate total
  total = calculate_total(coffe, muffin, donus, cookie)

  # show total
  print (f"Total need to pay : ${total: .2f}")

main()
