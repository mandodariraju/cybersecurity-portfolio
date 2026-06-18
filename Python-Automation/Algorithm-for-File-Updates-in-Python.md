# Algorithm for File Updates in Python

## Project Description

As a security professional working for a healthcare organization, I was tasked with maintaining an allow list of IP addresses authorized to access a restricted network containing sensitive patient information. The organization also maintained a remove list containing IP addresses that should no longer have access to the network.

To automate this process, I developed a Python algorithm that opens the allow list file, reads its contents, removes unauthorized IP addresses found in the remove list, and updates the file with the revised list. This project demonstrates file handling, data processing, iteration, conditional logic, and list manipulation using Python.

---

## Open the File That Contains the Allow List

### Code

```python
import_file = "allow_list.txt"

with open(import_file, "r") as file:
```

### Explanation

The variable `import_file` stores the name of the file containing the allow list. The `open()` function is used to open the file in read mode (`"r"`). A `with` statement is used to ensure that the file is automatically closed after the block of code finishes executing. The file object is stored in the variable `file`.

---

## Read the File Contents

### Code

```python
ip_addresses = file.read()
```

### Explanation

The `.read()` method reads the entire contents of the file and stores them as a string in the variable `ip_addresses`. This allows the program to access and process the data contained within the file.

---

## Convert the String into a List

### Code

```python
ip_addresses = ip_addresses.split()
```

### Explanation

The `.split()` method converts the string of IP addresses into a list. Each IP address becomes an individual list element, making it easier to search, modify, and remove entries as needed.

---

## Iterate Through the Remove List

### Code

```python
for element in remove_list:
```

### Explanation

A `for` loop is used to iterate through every IP address stored in the `remove_list`. The loop variable `element` represents one IP address at a time during each iteration.

---

## Remove IP Addresses That Are on the Remove List

### Code

```python
for element in remove_list:
    if element in ip_addresses:
        ip_addresses.remove(element)
```

### Explanation

The conditional statement checks whether the current IP address stored in `element` exists in the `ip_addresses` list. If it exists, the `.remove()` method deletes that IP address from the allow list.

This approach works because the `ip_addresses` list contains no duplicate entries. Therefore, removing a matching IP address once is sufficient.

---

## Update the File with the Revised List of IP Addresses

### Code

```python
ip_addresses = "\n".join(ip_addresses)

with open(import_file, "w") as file:
    file.write(ip_addresses)
```

### Explanation

The `.join()` method converts the list back into a string. The newline character (`"\n"`) ensures that each IP address appears on its own line in the updated file.

The file is then reopened using write mode (`"w"`). The `.write()` method replaces the contents of the file with the updated list of authorized IP addresses.

---

## Summary

This project demonstrates how Python can be used to automate security administration tasks involving file management and access control. The algorithm opens and reads an allow list file, converts the contents into a list, and iterates through a remove list to identify unauthorized IP addresses. Matching addresses are removed using conditional logic and list methods. Finally, the updated list is converted back into a string and written to the original file. This automation helps improve efficiency, accuracy, and consistency when managing network access permissions.
