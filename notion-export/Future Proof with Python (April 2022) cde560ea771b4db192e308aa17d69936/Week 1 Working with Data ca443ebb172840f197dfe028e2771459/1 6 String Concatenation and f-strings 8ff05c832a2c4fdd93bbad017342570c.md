# 1.6 String Concatenation and f-strings

*Estimated Time: 30 minutes*

---

### Key ideas

- Using formatted strings

## String Concatenation and f-strings

When there’s a variable we want to combine with a string to print out a message, so far we’ve added the strings with `+`.

```python
name = "Mercy"
print("Hello, " + name) # Hello, Mercy 
```

When the message is longer, this becomes more confusing and harder to type.

```python
name = "Mercy"
print("The alarm went off at exactly 6:00 AM as it had every morning for the past five years. " + name + " began her morning and was ready to eat breakfast by 7:00 AM. The day appeared to be as normal as any other, and " + name + " was not expecting anything to change.")
```

There’s another way to format long text that uses variables, called **f-strings.**

```python
name = "Mercy"
print(f"Hello, {name}") # Hello, Mercy
print(f"The alarm went off at exactly 6:00 AM as it had every morning for the past five years. {name} began her morning and was ready to eat breakfast by 7:00 AM. The day appeared to be as normal as any other, and {name} was not expecting anything to change.")
```

Instead of using `+` to combine the variable and the string, we start the string with `f` and we use `{}` to insert the variable right inside the string. That way, there’s less confusion about quote marks and spaces.

### Other f-string uses

We can also use f-strings for rounding.

```python
one_third = 1/3
print(one_third)# 0.3333333333333333
print(f"{one_third:.2}") # 0.33
```

f-strings have other formatting powers, but we’ll leave it at rounding floats for now.

## Practice: f-strings

<aside>
👩🏿‍💻 Practice using f-strings to format results.

</aside>

[https://replit.com/team/kibo-fpwp5/W15-F-strings-Practice](https://replit.com/team/kibo-fpwp5/W15-F-strings-Practice)

- Solution: **F-strings practice**
    
    ```python
    first_num = float(input("enter first number: "))
    second_num = float(input("enter second number: "))
    
    # change the line below
    result = first_num / second_num
    
    print(f"the result is {result:.3} ")
    ```
    

<aside>
<img src="../Lesson%200%20Learning%20With%20Kibo%2032002756da8b4ed2a610df0347af2a08/man-in-hike.png" alt="../Lesson%200%20Learning%20With%20Kibo%2032002756da8b4ed2a610df0347af2a08/man-in-hike.png" width="40px" /> Next up: [Practice](Practice%2038433a875ab64a918c1f21e1b958f20d.md)

</aside>