# Zoo-Animal-Inventory
Taking inventory of animals at the zoo. One by one, count the animals at a small zoo to record their numbers by animal type, as well as total number of animals at the zoo.
def get_animal_count(animal_name):
  """
  Gets the number of animals of a given type from the user.

  Args:
    animal_name: The name of the animal.

  Returns:
    The number of animals of the given type.
  """
  while True:
    try:
      count = int(input(f"Enter the number of {animal_name}: "))
      if count >= 0:
        return count
      else:
        print("Please enter a non-negative number.")
    except ValueError:
      print("Invalid input. Please enter a number.")

# Get animal counts from the user
zebras = get_animal_count("zebras")
flamingos = get_animal_count("flamingos")
tigers = get_animal_count("tigers")
lions = get_animal_count("lions")
peacocks = get_animal_count("peacocks")
capuchin_monkeys = get_animal_count("capuchin monkeys")
macaws = get_animal_count("macaws")

# Calculate total number of animals
total_animals = zebras + flamingos + tigers + lions + peacocks + capuchin_monkeys + macaws

# Print the inventory
print("\nZoo Animal Inventory:")
print(f"Zebras: {zebras}")
print(f"Flamingos: {flamingos}")
print(f"Tigers: {tigers}")
print(f"Lions: {lions}")
print(f"Peacocks: {peacocks}")
print(f"Capuchin Monkeys: {capuchin_monkeys}")
print(f"Macaws: {macaws}")
print(f"Total Animals: {total_animals}")
