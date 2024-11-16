Day-5
# PyPassword Generator 🔒

Welcome to the **PyPassword Generator**! This is a simple yet powerful tool to create strong and secure passwords to keep your online accounts safe.

## Project Description

The **PyPassword Generator** allows users to create highly secure passwords by including a mix of **letters**, **numbers**, and **symbols**. You can customize the length and complexity of your password based on your needs, making it a versatile tool for enhancing your account security.

## Features

- **Customizable Password Length**: Choose the number of letters, numbers, and symbols.
- **Strong Password Generation**: Combines uppercase and lowercase letters, digits, and special characters.
- **Randomization**: Uses Python's `random` module to shuffle the characters and enhance password security.
- **User-Friendly**: Simple and interactive command-line interface.

## How to Use

1. Clone the repository or copy the code into your Python environment.
2. Run the Python script.
3. You will be prompted to:
   - Enter the number of **letters** you want in your password.
   - Enter the number of **symbols** (e.g., `!`, `@`, `#`).
   - Enter the number of **numbers** (e.g., `1`, `2`, `3`).
4. The program will generate a random, secure password based on your inputs and display it.

### Example

```
Welcome to the PyPassword Generator!
How many letters would you like in your password?
6
How many symbols would you like?
3
How many numbers would you like?
4
Your password is: aB!3&g7H@5J
```

## Prerequisites

- Python 3.x installed on your system.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/aditya-kr86/password_generator.git
   ```

2. **Navigate to the project folder**:
   ```bash
   cd PasswordGenerator
   ```

3. **Run the script**:
   ```bash
   python password_generator.py
   ```

## Code Explanation

- The program uses three lists to store potential characters:
  - `letters`: Contains both uppercase and lowercase English alphabets.
  - `numbers`: Contains digits from `0` to `9`.
  - `symbols`: Contains special characters like `!`, `#`, `$`, etc.

- The user inputs the desired number of letters, symbols, and numbers for the password.
- The script generates a list of randomly selected characters based on the user's input.
- The `random.shuffle()` function is used to randomize the order of characters in the list.
- Finally, the list is converted to a string and displayed as the generated password.

### Code Structure

```python
# Generate a list of random letters
for char in range(1, nr_letters + 1):
  password_list.append(random.choice(letters))

# Generate a list of random symbols
for char in range(1, nr_symbols + 1):
  password_list.append(random.choice(symbols))

# Generate a list of random numbers
for char in range(1, nr_numbers + 1):
  password_list.append(random.choice(numbers))

# Shuffle the characters and create the final password
random.shuffle(password_list)
password = "".join(password_list)
print(f"Your password is: {password}")
```

## Project Structure

```
PasswordGenerator/
├── README.md
└── password_generator.py
```

## Contributing

Contributions are welcome! If you have any suggestions for improving the password generator, feel free to fork the repository and submit a pull request.

## Author

- [Aditya Kumar](https://github.com/aditya-kr86)

## License

This project is open-source and available under the MIT License.

## Feedback

If you have any feedback or suggestions, please reach out via [email](mailto:adityakumargupta082003@gmail.com).
