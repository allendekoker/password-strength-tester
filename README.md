# Password Strength Checker

This is a Python script that checks the strength of a given password based on certain rules.

## Usage

To use the password strength checker, follow these steps:

1. Import the script using `import password_strength`.
2. Call the `password_strength` function with the password to be checked as the argument.
3. The function returns a message indicating whether the password is strong or weak based on the defined rules.

## Password Strength Rules

The password strength rules are defined in the `rules` dictionary. The following rules are checked:

- **Length:** The password must be at least a certain length, as defined by the `length` key in the `rules` dictionary.
- **Lowercase Characters:** The password must contain at least one lowercase letter, as defined by the `lower` key in the `rules` dictionary.
- **Uppercase Characters:** The password must contain at least one uppercase letter, as defined by the `upper` key in the `rules` dictionary.
- **Digits:** The password must contain at least one digit, as defined by the `digit` key in the `rules` dictionary.
- **Special Characters:** The password must contain at least one special character, as defined by the `special` key in the `rules` dictionary.

## Example

```python
import password_strength

# define password to be checked
password = 'MyPassword123!'

# check password strength
result = password_strength.password_strength(password)

# print result
print(result)
```

This will output `Password is strong.` if the password meets all of the defined rules, or `Password is weak.` along with a message describing which rules were not met.