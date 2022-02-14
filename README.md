# calculator-app

getDisplayNumber(number) {
// function add comma after every three digits in our output
const floatNumber = parseFloat(number); //converts string to a floating number
if (isNaN(floatNumber)) return "";
return floatNumber.toLocaleString("en");
}

using this function does add comma after every three
digits however,

1.  we cannot start the number with decimal
    becase we have isNaN in our if statement, hence it sets it
    to empty string,
2.  we cannot type more than three digits after the decimal here

Hence, we need to split the number in two parts

integer - before the decimal place
decimal - comes after the decimal place
