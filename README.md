def greet(name):
    """
    This function greets the user by name.

    Args:
        name (str): The name of the user.

    Returns:
        str: A greeting message.
    """
    return f"Hello, {name}! Welcome to our program."

# Example usage:
user_name = "John"
greeting = greet(user_name)
print(greeting)
