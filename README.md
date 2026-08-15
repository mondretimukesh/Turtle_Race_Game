# 🐢 Turtle Race Game

A simple **Turtle Race Game** built using Python's `turtle` module. The player selects a turtle color and watches six colored turtles race toward the finish line. The program randomly moves each turtle until one reaches the finish line.

## 🎮 Features

* 🐢 Six colored turtles participate in the race.
* 🎨 Available colors:

  * Violet
  * Red
  * Blue
  * Green
  * Yellow
  * Orange
* 🎯 Players can bet on one turtle before the race starts.
* ⏱️ Countdown from **3 → 2 → 1 → GO!**
* 🎲 Each turtle moves a random distance on every turn.
* 🏆 The first turtle to cross the finish line wins.
* ✅ Displays **YOU WON!** if the player's chosen turtle wins.
* ❌ Displays **YOU LOST!** if another turtle wins.

## 🛠️ Technologies Used

* **Python 3**
* **Turtle Graphics**
* **Random Module**

Both `turtle` and `random` are part of Python's standard library, so no external packages are required.

## 📂 Project Structure

```text
Turtle-Race/
│
├── main.py
└── README.md
```

## ▶️ How to Run

### 1. Install Python

Make sure Python 3 is installed on your system.

Check your Python version:

```bash
python --version
```

### 2. Run the program

Save the code as `main.py` and run:

```bash
python main.py
```

A Turtle graphics window will open.

### 3. Place Your Bet

A dialog box will ask you to choose a turtle color.

Example:

```text
Place your bets on the following colored turtles:
['violet', 'red', 'blue', 'green', 'yellow', 'orange']
```

Enter one of the available colors.

## 🕹️ How the Game Works

1. Six turtles are created.

2. Each turtle is assigned a different color.

3. The turtles are positioned at the starting line.

4. A countdown appears:

   **3 → 2 → 1 → GO!**

5. Each turtle moves a random distance between `0` and `10` pixels.

6. The race continues until one turtle crosses the finish line.

7. The winning turtle is identified.

8. The program compares the winner with the player's selected color.

9. The result is displayed as either:

   **YOU WON!** or **YOU LOST!**

## 🧠 Important Python Concepts Used

### Random Movement

```python
each_distance = random.randint(0, 10)
turtles.forward(each_distance)
```

Generates a random distance between 0 and 10 pixels for every turtle.

### Detecting the Winner

```python
if turtles.xcor() > 230:
    is_race_on = False
    winner_turtle = turtles.fillcolor()
```

The race stops when a turtle crosses the finish line.

### User Input

```python
user_color = screen.textinput(
    "Turtle Race",
    "Place your bets on the following colored turtles..."
).lower()
```

Gets the player's selected turtle color.

## 🏆 Example Output

If the player chooses:

```text
blue
```

and the blue turtle wins:

```text
YOU WON!
blue Won the RACE!
```

If another turtle wins:

```text
YOU LOST!
red Won the RACE!
```

## 📌 Requirements

* Python 3.x
* A computer with graphical display support
* No external Python libraries required

## 🚀 Future Improvements

Some possible improvements include:

* Add a visible finish line.
* Add turtle names instead of only colors.
* Add multiple rounds.
* Keep track of the player's score.
* Add sound effects.
* Add a restart button.
* Improve the countdown display.
* Add a graphical betting interface.
* Display the race results in a more attractive format.

## 👨‍💻 Author

**Mondreti Mukesh**

A beginner-friendly Python project created to practice:

* Python basics
* Loops
* Conditional statements
* Functions/modules
* Random numbers
* User input
* Turtle graphics
