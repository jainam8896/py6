n=int(input("How many Number You Want to Enter"))

my_list = []

for i in range(n):

    no = input("Enter a number: ")

    my_list.append(no)

while True:

    print("Enter 1 to count the total number of elements in the list")

    print("Enter 2 to count the total number of vowels in the list")

    print("Enter 3 to count the total number of consonants in the list")

    print("Enter 4 to count the total number of other characters in the list")

    print("Enter 5 to Print the list")

    print("Enter 6 to exit the program")

    

    choice = int(input("Enter your choice: "))

    

    if choice == 1:

        print("Total number of elements in the list:", len(my_list))

    elif choice == 2:

        vowel_count = 0

        for character in my_list:

            if character in ['a', 'e', 'i', 'o', 'u', 'A', 'E', 'I', 'O', 'U']:

                vowel_count += 1

        print("Total number of vowels in the list:", vowel_count)

    elif choice == 3:

        consonant_count = 0

        for character in my_list:

            if character.isalpha() and character not in ['a', 'e', 'i', 'o', 'u', 'A', 'E', 'I', 'O', 'U']:

                consonant_count += 1

        print("Total number of consonants in the list:", consonant_count)

    elif choice == 4:

        other_count = 0

        for character in my_list:

            if not character.isalpha() and not character.isdigit():

                other_count += 1

        print("Total number of other characters in the list:", other_count)

    elif choice == 5:

        for j in my_list:

            print(j)

        

    elif choice == 6:

        print("Exiting the program...")

        break

    else:

        print("Invalid choice! Please enter a valid choice.")
