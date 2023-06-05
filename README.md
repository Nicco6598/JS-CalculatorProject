# JSCalculator

![Alt text](/images/screenshotJS.jpg "JSCalculator index")

JSCalculator is a JavaScript calculator that increases/resets/decreases the displayed value on the screen."

With JSCalculator, users can easily manipulate numerical values by employing the intuitive controls provided. By selecting the "increase" function, the calculator will increment the displayed value, allowing users to add to the existing total effortlessly. This feature is particularly useful when performing calculations that involve incremental values or when tracking progressive changes.

On the other hand, the "reset" function allows users to revert the displayed value back to its original state, erasing any modifications made. This feature is handy in situations where a user wants to start fresh or discard any previous calculations.

Additionally, JSCalculator provides the option to "decrease" the displayed value. This functionality allows users to subtract from the existing total, facilitating calculations involving deductions or reducing values. This feature is especially valuable when working with variables that require step-by-step reduction.

Overall, JSCalculator offers a user-friendly interface and powerful functionalities to enhance mathematical operations. Whether you need to increase, reset, or decrease values, this JavaScript calculator provides a convenient and efficient solution for manipulating numerical data on the screen.

## Installation

Use the Git Bash terminal to clone the repository locally.

```gitbash
git clone https://github.com/Nicco6598/JS-CalculatorProject.git
```

## Index.html buttons and counter

```html
<label id="countLabel">0</label><br>
    <div class="container">
        <div class="vertical-center"></div>
            <button id="decreaseBtn">decrease</button>
            <button id="resetBtn">reset</button>
            <button id="increaseBtn">increase</button>
            <script src="js/index.js"></script>
        </div>
    </div>
```

## Index.js functions

```js
let count = 0;

document.getElementById("decreaseBtn").onclick = function(){
    count-=1;
    document.getElementById("countLabel").innerHTML = count;
}

document.getElementById("resetBtn").onclick = function(){
    count=0;
    document.getElementById("countLabel").innerHTML = count;
}

document.getElementById("increaseBtn").onclick = function(){
    count+=1;
    document.getElementById("countLabel").innerHTML = count;
}
```

## License

[MIT](https://github.com/Nicco6598/JS-CalculatorProject/blob/main/license.txt)