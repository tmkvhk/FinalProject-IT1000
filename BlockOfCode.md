# Code Example
## This is an example of some of the coding I have learned how to do this semester thanks to IT 1000
```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Fizz Buzz</title>
<script>

function fizzbuzz() {
	var display = document.getElementById('display');
	var displayHTML = "";
	for (i = 0; i < 100; i++) {
		displayHTML += "<p>" + i + "</p>";
	}
	display.innerHTML = displayHTML;
}

</script>

</head>

<body onload="fizzbuzz()">
<div id="display">

</div>
</body>

</html>
```

### This was one of coding assignment from earlier in the year. It is a cylinder coating estimator.
```python
import math
def getfloat(prompt):
    while True:
        try:
            value=float(input(prompt))
            if value < 0:
                print("Please enter a Positive Number")
                continue
        except ValueError:
            print("The input is not a valid floating point number. Please re-enter.")
        else:
            break
    return value
def docalculation():
    radius = getfloat("What is the Radius?")
    height = getfloat("What is the Height?")
    coating= getfloat("What is the cost of the coating?")

    final_area = 2 * math.pi * radius * height + 2 * math.pi * radius * radius
    pints = final_area/50
    total_cost = round(pints) * coating

    print("The Surface Area is", final_area)
    print("{} pints are required costing ${:,.2f}.".format(round(pints), total_cost))

def main():
    while True:
        docalculation()
        recalculate = input("Would you like to do another calculation? (y/n)? ")
        if(recalculate != "y"):
            break


main()
```
[return to home page](./README.md)


