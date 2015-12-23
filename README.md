# py-timed-dialog
Create dialog boxes that self destruct after a set period of time.

## Installing the package

#### Python 2

```
pip install py-timed-dialog
```

#### Python 3

```
pip3 install py-timed-dialog
```

## Importing the class

```python
from ptd import TimedDialog
```

## Button input

```python
async = TimedDialog()
value = async.button_input(
          title='Title!',
          message='Perform this action?',
          buttons={1: "Yes", 2: "No", "maybe": "Maybe"},
          default=1,
          timeout=3000
        )
print(value)
```

Output:

```
1       # Or the key of the button pressed in case the user clicks on a button
```
