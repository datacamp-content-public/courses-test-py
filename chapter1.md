---
title: 'Chapter Title Here'
description: 'Chapter description goes here.'
---

## Insert exercise title here

```yaml
type: DragAndDropExercise
key: 616239cb78
kind: Order
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Instruction 1
- Instruction 2

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@solution`
```{python}
# Edit or remove this code to create your own exercise.
# This is 1 type of drag and drop exercise, there are 2 other types. See documentation:
# http://instructor-support.datacamp.com/en/articles/3039539-course-drag-drop-exercises

# Make sure you only use SPACES, NOT TABS in front of each line.
- id: data_science_process
  title: Data Science Process
  items:
    - id: question # ID of the item. This can be used in the SCTs.
      content: Ask an interesting question # Name of an item. Feel free to use markdown.
    - id: data
      content: Get the data
    - id: explore
      content: Explore the data
    - id: model
      content: Model the data
    - id: communicate
      content: Communicate and visualize the results
```

`@sct`
```{python}
checks:
  - condition: check_index(question) == solution
    incorrectMessage: 'Wrong! Try again!' # If that condition is not true, show this message.
  - condition: check_index(data) == solution
    incorrectMessage: 'Try again! You can do it!'
  - condition: check_index(explore) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(model) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(communicate) == solution
    incorrectMessage: 'We believe in you, try again!'
successMessage: "Congratulations" # Message shown when all is correct.
failureMessage: "Try again!" # Message shown when there are errors (and there is no specific error available).
isOrdered: true # Should the items in the zones be ordered as in the solution code?
```

---

## Insert exercise title here

```yaml
type: VideoExercise
key: 4612298727
xp: 50
```

`@projector_key`
46960d511eeda7f8975d21bc689254b4

---

## Insert exercise title here

```yaml
type: DragAndDropExercise
key: 92715d8ff9
kind: Classify
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Instruction 1
- Instruction 2

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@solution`
```{python}
# Edit or remove this code to create your own exercise.
# This is 1 type of drag and drop exercise, there are 2 other types. See documentation:
# http://instructor-support.datacamp.com/en/articles/3039539-course-drag-drop-exercises

# Make sure you only use SPACES, NOT TABS in front of each line.

# Drag zone that holds all the options.
# Specify an ID for this zone to use in SCTs.
- id: options
  title: "Options" # Title of your zone This is not shown with more than 2 zones.

# You can keep adding drop zones to sort to.
# This example has 2 zones.
- id: dropzone_r
  title: "R"
  items: # Each drop zone has a list of items it contains. These will be shown in a random fashion.
    - content: "stringr" # Name of an item. Feel free to use markdown.
      id: stringr # ID of the item. This can be used in the SCTs.
    - content: "dplyr"
      id: dplyr

- id: dropzone_python
  title: "Python"
  items:
    - content: "pandas"
      id: pandas
    - content: "numpy"
      id: numpy
    
```

`@sct`
```{python}
checks: # Individual checks and custom messages per item. This is optional. Without it, it will check that the options are as in the solution code.
  - condition: check_target(pandas) == dropzone_python # Check that pandas is in dropzone_python.
    incorrectMessage: 'Hmm! Pandas is a Python package.' # If that condition is not true, show this message.
  - condition: check_target(numpy) == dropzone_python
    incorrectMessage: 'Damn, this is far from perfect!'
  - condition: check_target(dplyr) == dropzone_r
    incorrectMessage: "Hmm, keep doing R courses! :-)"
  - condition: check_target(stringr) == dropzone_r
    incorrectMessage: "How funny if stringr would be a Python package."
successMessage: "Congratulations" # Message shown when all is correct.
failureMessage: "Try again!" # Message shown when there are errors (and there is no specific error available).
isOrdered: false # Should the items in the zones be ordered as in the solution code?
```

---

## Insert exercise title here

```yaml
type: DragAndDropExercise
key: a50ec0c11b
kind: Order
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Instruction 1
- Instruction 2

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@solution`
```{python}
# Edit or remove this code to create your own exercise.
# This is 1 type of drag and drop exercise, there are 2 other types. See documentation:
# http://instructor-support.datacamp.com/en/articles/3039539-course-drag-drop-exercises

# Make sure you only use SPACES, NOT TABS in front of each line.
- id: data_science_process
  title: Data Science Process
  items:
    - id: question # ID of the item. This can be used in the SCTs.
      content: Ask an interesting question # Name of an item. Feel free to use markdown.
    - id: data
      content: Get the data
    - id: explore
      content: Explore the data
    - id: model
      content: Model the data
    - id: communicate
      content: Communicate and visualize the results
```

`@sct`
```{python}
checks:
  - condition: check_index(question) == solution
    incorrectMessage: 'Wrong! Try again!' # If that condition is not true, show this message.
  - condition: check_index(data) == solution
    incorrectMessage: 'Try again! You can do it!'
  - condition: check_index(explore) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(model) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(communicate) == solution
    incorrectMessage: 'We believe in you, try again!'
successMessage: "Congratulations" # Message shown when all is correct.
failureMessage: "Try again!" # Message shown when there are errors (and there is no specific error available).
isOrdered: true # Should the items in the zones be ordered as in the solution code?
```

---

## Insert exercise title here

```yaml
type: MultipleChoiceExercise
key: c0a8b5ce88
xp: 50
```

<!-- Guidelines for the question: https://instructor-support.datacamp.com/en/articles/2375523-course-multiple-choice-with-console-exercises. -->

`@possible_answers`
- [Correct answer 1]
- Wrong answer 2
- Wrong answer 3

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@pre_exercise_code`
```{python}

```

`@sct`
```{python}
# Check https://instructor-support.datacamp.com/en/articles/2375523-course-multiple-choice-with-console-exercises on how to write feedback messages for this exercise.
```

---

## Insert exercise title here

```yaml
type: PureMultipleChoiceExercise
key: 88bf1d8567
xp: 50
```

<!-- Guidelines for the question: https://instructor-support.datacamp.com/en/articles/2375516-course-multiple-choice-exercises. -->

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@possible_answers`
- [Correct answer 1]
- Wrong answer 2
- Wrong answer 3

`@feedback`
<!-- Examples of good feedback messages: https://instructor-support.datacamp.com/en/articles/2299773-exercise-success-messages.  -->
- Perfect!
- Error message answer 2
- Error message answer 3

---

## Insert exercise title here

```yaml
type: TabExercise
key: 0d73731ba6
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375525-course-sequential-exercises. -->

`@pre_exercise_code`
```{python}

```

---

## Insert exercise title here

```yaml
type: BulletExercise
key: 1d96a70379
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375528-course-iterative-exercises -->

`@pre_exercise_code`
```{python}

```

---

## Insert exercise title here

```yaml
type: BulletExercise
key: f38c96718b
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375528-course-iterative-exercises -->

`@pre_exercise_code`
```{python}

```

---

## Insert exercise title here

```yaml
type: DragAndDropExercise
key: 36cabccbb1
kind: Classify
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Instruction 1
- Instruction 2

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@solution`
```{python}
# Edit or remove this code to create your own exercise.
# This is 1 type of drag and drop exercise, there are 2 other types. See documentation:
# http://instructor-support.datacamp.com/en/articles/3039539-course-drag-drop-exercises

# Make sure you only use SPACES, NOT TABS in front of each line.

# Drag zone that holds all the options.
# Specify an ID for this zone to use in SCTs.
- id: options
  title: "Options" # Title of your zone This is not shown with more than 2 zones.

# You can keep adding drop zones to sort to.
# This example has 2 zones.
- id: dropzone_r
  title: "R"
  items: # Each drop zone has a list of items it contains. These will be shown in a random fashion.
    - content: "stringr" # Name of an item. Feel free to use markdown.
      id: stringr # ID of the item. This can be used in the SCTs.
    - content: "dplyr"
      id: dplyr

- id: dropzone_python
  title: "Python"
  items:
    - content: "pandas"
      id: pandas
    - content: "numpy"
      id: numpy
    
```

`@sct`
```{python}
checks: # Individual checks and custom messages per item. This is optional. Without it, it will check that the options are as in the solution code.
  - condition: check_target(pandas) == dropzone_python # Check that pandas is in dropzone_python.
    incorrectMessage: 'Hmm! Pandas is a Python package.' # If that condition is not true, show this message.
  - condition: check_target(numpy) == dropzone_python
    incorrectMessage: 'Damn, this is far from perfect!'
  - condition: check_target(dplyr) == dropzone_r
    incorrectMessage: "Hmm, keep doing R courses! :-)"
  - condition: check_target(stringr) == dropzone_r
    incorrectMessage: "How funny if stringr would be a Python package."
successMessage: "Congratulations" # Message shown when all is correct.
failureMessage: "Try again!" # Message shown when there are errors (and there is no specific error available).
isOrdered: false # Should the items in the zones be ordered as in the solution code?
```

---

## Insert exercise title here

```yaml
type: DragAndDropExercise
key: 250f9e5d18
kind: Order
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Instruction 1
- Instruction 2

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@solution`
```{python}
# Edit or remove this code to create your own exercise.
# This is 1 type of drag and drop exercise, there are 2 other types. See documentation:
# http://instructor-support.datacamp.com/en/articles/3039539-course-drag-drop-exercises

# Make sure you only use SPACES, NOT TABS in front of each line.
- id: data_science_process
  title: Data Science Process
  items:
    - id: question # ID of the item. This can be used in the SCTs.
      content: Ask an interesting question # Name of an item. Feel free to use markdown.
    - id: data
      content: Get the data
    - id: explore
      content: Explore the data
    - id: model
      content: Model the data
    - id: communicate
      content: Communicate and visualize the results
```

`@sct`
```{python}
checks:
  - condition: check_index(question) == solution
    incorrectMessage: 'Wrong! Try again!' # If that condition is not true, show this message.
  - condition: check_index(data) == solution
    incorrectMessage: 'Try again! You can do it!'
  - condition: check_index(explore) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(model) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(communicate) == solution
    incorrectMessage: 'We believe in you, try again!'
successMessage: "Congratulations" # Message shown when all is correct.
failureMessage: "Try again!" # Message shown when there are errors (and there is no specific error available).
isOrdered: true # Should the items in the zones be ordered as in the solution code?
```

---

## Insert exercise title here

```yaml
type: DragAndDropExercise
key: f1c39a7728
kind: Order
xp: 100
```

<!-- Guidelines for contexts: https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->

`@instructions`
<!-- Guidelines for instructions https://instructor-support.datacamp.com/en/articles/2375526-course-coding-exercises. -->
- Instruction 1
- Instruction 2

`@hint`
<!-- Examples of good hints: https://instructor-support.datacamp.com/en/articles/2379164-hints-best-practices. -->
- This is an example hint.
- This is an example hint.

`@solution`
```{python}
# Edit or remove this code to create your own exercise.
# This is 1 type of drag and drop exercise, there are 2 other types. See documentation:
# http://instructor-support.datacamp.com/en/articles/3039539-course-drag-drop-exercises

# Make sure you only use SPACES, NOT TABS in front of each line.
- id: data_science_process
  title: Data Science Process
  items:
    - id: question # ID of the item. This can be used in the SCTs.
      content: Ask an interesting question # Name of an item. Feel free to use markdown.
    - id: data
      content: Get the data
    - id: explore
      content: Explore the data
    - id: model
      content: Model the data
    - id: communicate
      content: Communicate and visualize the results
```

`@sct`
```{python}
checks:
  - condition: check_index(question) == solution
    incorrectMessage: 'Wrong! Try again!' # If that condition is not true, show this message.
  - condition: check_index(data) == solution
    incorrectMessage: 'Try again! You can do it!'
  - condition: check_index(explore) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(model) == solution
    incorrectMessage: 'We believe in you, try again!'
  - condition: check_index(communicate) == solution
    incorrectMessage: 'We believe in you, try again!'
successMessage: "Congratulations" # Message shown when all is correct.
failureMessage: "Try again!" # Message shown when there are errors (and there is no specific error available).
isOrdered: true # Should the items in the zones be ordered as in the solution code?
```
