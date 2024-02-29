# cis129_lab03_coffeeShop.py
print("My Coffee and Muffin Shop")

print("Menu of My Coffee and Muffin Shop")
print("1 Coffee at $5 each")
print("2 Muffins at $4 each")
print("6% tax")

def calculate_total(coffe, muffin):
  # calculate 
  coffe_price = 5
  muffin_price = 4
  subtotal = (coffe * coffe_price) + (muffin * muffin_price)

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

  # calculate total
  total = calculate_total(coffe, muffin)

  # show total
  print (f"Total need to pay : ${total: .2f}")

main()
