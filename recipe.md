## 1. Describe the Problem

As a user
So I don't forget the details
I want to keep a record of friends' names and birthdates

As a user
So I can make edits when I've got dates wrong
I want to be able to update a record by passing in a name and new date

As a user
So I can make edits when people change their name
I want to be able to update a record by passing in an old and a new name

As a user
So I can remember to send birthday cards at the right time
I want to be able to list friends whose birthdays are coming up soon and to whom I need to send a card

As a user
So I can buy age-appropriate birthday cards
I want to calculate the upcoming ages for friends with birthdays

## 2. Design the Class Interface

```python

from datetime import date

class Friend:

    def __init__(self, name, birthday):
        # Parameters:
        #   self.name (string) and self.birthday (date) to store names / dobs
        # Side effects:
        #   None
        # Returns:
        #   None
        self.name = name
        self.birthday = birthday

    def update_name(self, new_name):
        # Parameters:
        #   new_name (string) to update name in Class
        # Side effects:
        #   Will update name in Class
        # Returns:
        #   None
        pass

    def update_birthday(self, new_birthday):
        # Parameters:
        #   new_birthday (date) to update birthday in Class
        # Side effects:
        #   Will update birthday in Class
        # Returns:
        #   None
        pass

    def upcoming_age(self, current_date):
        # Parameters:
        #   current_date (date) to calculate today's date and compare with dob
        # Side effects:
        #   None
        # Returns:
        #   None
        pass


class BirthdayReminder:

    def __init__(self):
        # Parameters:
        #   None
        # Side effects:
        #   None
        # Returns:
        #   None
        self.friends = []

    def add(self, friend):
        # Parameters:
        #   friend: instance of Friend()
        # Side effects:
        #   self.friends amended
        # Returns:
        #   None
        pass

    def update_friend_date(self, name, new_birthday):
        # Parameters:
        #   name (string) for friend's name
        #   new_birthday (date) to amend friend's dob
        # Side effects:
        #   self.friends amended
        # Returns:
        #   None        
        pass

    def update_friend_name(self, old_name, new_name):
        # Parameters:
        #   old_name (string) for friend's previous name
        #   new_name (string) for friend's new name
        # Side effects:
        #   self.friends will be amended to change old name to new
        # Returns:
        #   None        
        pass

    def get_upcoming_birthdays(self, current_date, days_ahead=30):
        # Parameters:
        #   current_date (date) to calculate friend's upcoming age
        #   days_ahead (int) to calculate dob from current date  
        # Side effects:
        #   None
        # Returns:
        #   List of birthdays that fall within a certain window (i.e. next 30 days)
        pass
```

## 3. Create Examples as Tests

``` python
# EXAMPLE


```

## 4. Implement the Behaviour