import random
pet_names = {
    "dog": ["Bruno", "Max", "Daisy"],
    "cat": ["Luna", "Kitty", "Simba"],
    "rabbit": ["Fluffy", "Thumper", "Snowy"],
    "bird": ["Sky", "Tweety", "Coco"]
}
def suggest_name(pet_type):
    return random.choice(pet_names[pet_type])
while True:
    pet_type = input("What type of pet do you have? (Dog/Cat/Rabbit/Bird): ").strip().lower()
    if pet_type not in pet_names:
        print("Sorry, that pet type is not recognized. Please enter Dog, Cat, Rabbit, or Bird.")
        continue
    name = suggest_name(pet_type)
    print(f"Suggested name for your {pet_type.capitalize()}: {name}")
    another = input("Do you want another name suggestion? (Yes/No): ").strip().lower()
    if another != "yes":
    print("Thank you for using the Pet Name Suggester Bot!")
        break

        
