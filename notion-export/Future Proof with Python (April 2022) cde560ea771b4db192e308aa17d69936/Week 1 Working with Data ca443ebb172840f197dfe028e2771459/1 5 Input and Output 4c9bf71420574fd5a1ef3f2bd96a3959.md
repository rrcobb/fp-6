# 1.5. Input and Output

*Estimated Time: 30 minutes*

---

### Key ideas

- Show output with `print()`
- Get data from the user with `input()`

## Printing Output

Websites and apps you have used in the past have a whole screen full of text and buttons. Eventually, you’ll learn to build those kinds of programs, but we’re starting with the basics: programs that work with text.

`print` shows some output to the Console:

```python
print("Hello, world")
```

You’ve written code like this from your first “Hello, World” program. When you run it, the output shows up. In Replit, output shows in the ‘Console’ tab. On early computers, there was *only* a text console. On the earliest computers, there wasn’t a screen at all - instead, the output was printed out on paper. The output now shows up in the Console in our web browser, but we still call the function `print`.

```python
print("We can print any string we want")
x = ("If the string is in a variable, we can print the variable")
print(x) # If the string is in a variable, we can print the variable
```

## Getting Input from the User

You've already used the `input()` function in earlier challenges to get the name from the user.

When Python sees `input`:

- It prints out the arguments to `input`, similar to `print`.
- It pauses to wait for the user to type something in
- It waits for the user to press Enter
- When the user presses Enter, `input` gives the program the text that the user typed in

We can design lots of text-based interactions using `input`. A calculator, a search engine, a quiz, a chatbot - all of these and more can be designed to use text input and output.

### Converting Inputs

The `input()` function returns a **string**. If you want a number, need to convert the data type using `int` or `float`.

```python
response = input("How old are you?")
age = int(response)
```

It’s common to see the input and the conversion all at once, like this:

```python
age = int(input("How old are you?"))
```

Converting to a float is similar:

```python
soda_price = float(input("How much does a soda cost?"))
```

- What does python do if you try to convert a string like `"3.5"` to an integer using `int`?
    
    ```python
    int("3.5") # ValueError: invalid literal for int() with base 10: '3.5'
    ```
    
    <aside>
    ⚠️ Python doesn’t want to accidentally lose information. Instead of guessing whether you want to round up or down, it raises a `ValueError` and halts the program.
    
    </aside>
    

### Practice: Assigning and printing user input

<aside>
👩🏿‍💻 Let's practice assigning and printing user input. Modify the code below by following the directions in the **Instructions** tab.

</aside>

[https://replit.com/team/kibo-fpwp5/Input-Hours-of-Sleep](https://replit.com/team/kibo-fpwp5/Input-Hours-of-Sleep)

<aside>
📌 Here's what the output should look like when you run the program

![1%205%20Input%20and%20Output%204c9bf71420574fd5a1ef3f2bd96a3959/Untitled.png](1%205%20Input%20and%20Output%204c9bf71420574fd5a1ef3f2bd96a3959/Untitled.png)

</aside>

## Experimenting With Print

```python
print()
print
print("Hello", "world")
```

What happens when there’s nothing between the parentheses? Or if you leave off the parentheses? Or if you put more than one thing between the parentheses?

Sometimes, the best way to find things out about how Python works is to try it out.

- **Experiment with `print` to find out what it does in different situations**
    
    [https://replit.com/@kibocurriculum/Explore-With-Print](https://replit.com/@kibocurriculum/Explore-With-Print)
    

## Print with multiple arguments

<aside>
ℹ️ **Function Arguments**

**`print` and `input` are **functions**. We haven’t talked much about what functions are yet. We can still use them without fully understanding them yet. 

The name of “the things between the parentheses” is ***arguments**.*

Function **arguments** let the same function do something different each time you use it. `print` always sends *something* to the Console, but what it sends depends on the *arguments* in the parentheses.

</aside>

The `print()` function can take more than one argument. It can have more than one thing inside the `(...)`

However, you must separate arguments by commas.

```python
name = "Emmy"
print("Hello" name) # SyntaxError: invalid syntax (because there's no comma)
print("Hello", name) # Hello Emmy
```

## **Example: Input and Output**

<aside>
👉🏿 Let's take a look at a Python program that gives instructions to add two numbers:

<aside>
👩🏿‍💻 Below is an embedded program from Replit. 

****To complete:**
(1) **Run** the code using the green "Run ▷" button
(2) **Follow** the prompts in the `Console` tab below, to enter two numbers
(3) **See** the results of the program

</aside>

[https://replit.com/@kibocurriculum/add-two-numbers](https://replit.com/@kibocurriculum/add-two-numbers)

In plain English, here is what the code does:

- **line 1:** Ask the user for an input. Convert the input to an integer, and store it in a variable named `first_num`
- **line 2:** Ask the user for another input. Convert the input to an integer, and store it in a variable named `second_num`
- **line 4:** Add `first_num` and `second_num` and put the result in a third variable named `total`
- **line 6:** Print out the string "the sum is" and the value of the variable named `total`

<aside>
🧑🏿‍🔬 **Explore some more!**
Try more inputs to the program. What happens if you enter something that's not a number?  What happens if you press enter without typing a number? What happens if you never enter anything?

</aside>

</aside>

## Practice: Add three numbers

<aside>
👩🏿‍💻 Update the code below to add three numbers and print the total. Modify the code below by following the directions in the **Instructions** tab.
**

</aside>

[https://replit.com/team/kibo-fpwp5/Add-Three-Numbers](https://replit.com/team/kibo-fpwp5/Add-Three-Numbers)

<aside>
🆘 If you have trouble solving this challenge:

1) Read the instructions again.
2) Remember **G**o **C**limb **K**ibo - first Google, then ask the Community on Discord, then reach out to Kibo instructional team.
3) Don't spend more than 10 minutes stuck on this problem. If you've spent more time than that, take a look at the solution below.

</aside>

- Solution: **Add Three Numbers**
    
    ```python
    first_num = int(input("enter first number: "))
    second_num = int(input("enter second number: "))
    third_num = int(input("enter third number: "))
    
    # change the line below
    total = first_num + second_num + third_num
    
    # edit the text that will show up
    print("the sum of the three numbers is: ", total)
    ```
    

<aside>
<img src="../Lesson%200%20Learning%20With%20Kibo%2032002756da8b4ed2a610df0347af2a08/man-in-hike.png" alt="../Lesson%200%20Learning%20With%20Kibo%2032002756da8b4ed2a610df0347af2a08/man-in-hike.png" width="40px" /> Next up: [String Concatenation and f-strings](1%206%20String%20Concatenation%20and%20f-strings%208ff05c832a2c4fdd93bbad017342570c.md)

</aside>