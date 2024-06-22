    def encrypt(text, shift):
    encrypted_text = ""
    for char in text:
        if char.isalpha():
            shift_amount = shift % 26
            new_char = chr(((ord(char.lower()) - 97 + shift_amount) % 26) + 97)
            if char.isupper():
                new_char = new_char.upper()
            encrypted_text += new_char
        else:
            encrypted_text += char
    return encrypted_text

    def decrypt(text, shift):
    decrypted_text = ""
    for char in text:
        if char.isalpha():
            shift_amount = shift % 26
            new_char = chr(((ord(char.lower()) - 97 - shift_amount) % 26) + 97)
            if char.isupper():
                new_char = new_char.upper()
            decrypted_text += new_char
        else:
            decrypted_text += char
    return decrypted_text

    def main():
    while True:
        choice = input("Do you want to (e)ncrypt or (d)ecrypt a message? (e/d): ").lower()
        if choice in ['e', 'd']:
            break
        print("Invalid choice. Please enter 'e' to encrypt or 'd' to decrypt.")

    message = input("Enter the message: ")
    while True:
        try:
            shift = int(input("Enter the shift value: "))
            break
        except ValueError:
            print("Invalid shift value. Please enter an integer.")

    if choice == 'e':
        result = encrypt(message, shift)
        print(f"Encrypted message: {result}")
    else:
        result = decrypt(message, shift)
        print(f"Decrypted message: {result}")

    if __name__ == "__main__":
    main()
