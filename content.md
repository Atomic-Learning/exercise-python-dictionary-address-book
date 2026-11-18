Create a nested dictionary address book to understand how complex data can be organized in Python.

# Instructions

1. Create a dictionary named `contacts` to store your address book
2. Add at least two entries to it, including one for Alice and one for Bob.
    * The key should be a person's name 
    * The value is itself a dictionary containing contact details
    * Those contact details should have keys: `"phone"`, `"address"`, and `"email"`
3. Print the entire contacts dictionary
4. Access and print individual contact details:
    * Print Alice's phone number
    * Print Bob's email address
5. Add a new contact with all three details
6. Update one contact's information (e.g., change a phone number)

Write your code in the cell below.

```py-cell
# Write your code here

```

# Sample Solution

Click below to see a sample solution.

>[!HIDDEN]
> First, we need to create our dictionary of contacts. Each contact will be a key, and the value will be another dictionary with their details.
>
> ```py-cell
> contacts = {
>    "Alice": {
>        "phone": "01234 567890",
>        "address": "10 Downing St, London",
>        "email": "alice@example.com"
>    },
>    "Bob": {
>        "phone": "07771 234567",
>        "address": "Buckingham Palace, London",
>        "email": "bob@example.com"
>    }
> }
> ```
>
> Let's print the entire contacts dictionary to see its structure.
>
> ```py-cell
> print(contacts)
> ```
>
> We can access individual pieces of information by using two sets of square brackets: first for the person, then for the detail we want.
>
> ```py-cell
> print(contacts["Alice"]["phone"])
> print(contacts["Bob"]["email"])
> ```
>
> Now, let's add a new contact to our dictionary. We'll add Charlie with all their details.
>
> ```py-cell
> contacts["Charlie"] = {
>     "phone": "0207 1234567",
>     "address": "Imperial College, London",
>     "email": "charlie@example.com"
> }
> print(contacts["Charlie"])
> ```
>
> Finally, we can update information for an existing contact. Here, we change Alice's phone number.
>
> ```py-cell
> contacts["Alice"]["phone"] = "07788 654321"
> print(contacts["Alice"]["phone"])
> ```
