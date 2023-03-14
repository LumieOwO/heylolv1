```python
class GitHub_user:
    def __init__(
        self,
        Github_username: str = "",
        interests: list = list(),
        currently_learning: list = list(),
        age: int = 0,
        location: str = "",
    ):
        """
        Args:
            Github_username (str): The name of the user.
            interests (list): The interests of the user.
            currently_learning (list): The things the user is currently learning.
            age (int): The age of the user.
            location (str): The location of the user.
        """
        self.name: str = Github_username
        self.interests: list = interests
        self.age: int = age
        self.currently_learning: list = currently_learning
        self.location: str = location

    def get_name(self) -> str:
        return str(f"My username is {self.name}")

    def get_age(self) -> str:
        return str(f"My age is {self.age}")

    def get_location(self) -> str:
        return str(f"My location is {self.location}")

    def get_interests(self) -> str:
        return str(f"My interests are {self.interests}")

    def get_currently_learning(self) -> str:
        return str(f"I'm currently learning {self.currently_learning}")

    def __str__(self, value) -> str:
        return str(value)

    def get_all_info(self) -> str:
        return self.__str__(
            f"{self.get_name()}\n
            {self.get_location()}\n
            {self.get_age()}\n
            {self.get_interests()}\n
            {self.get_currently_learning()}"
        )


if __name__ == "__main__":
    heylol = GitHub_user(
        Github_username="Lumie",
        interests=[
            "coding",
            "python",
        ],
        currently_learning=[
        "python",
        ],
        age=13,
        location="Israel",
    )
heylol.get_all_info()
```
