# Mobile number keyboard & only Number Validation
This plugin or code is created to avoid alpha keyboard and alphabets to write in the input number or tel type. So, for avoiding we'll use jquery. Here we go....
## Installation
First add below jquery in your footer, so it will work on all fields
```jquery
$(document).on("input", "input[type='tel']", function() {
    this.value = this.value.replace(/\D/g,'');
});

// OR

$(".numericOnly").keypress(function (e) {
    if (String.fromCharCode(e.keyCode).match(/[^0-9]/g)) return false;
});
```
Now, you can add this class ```.numericOnly``` to any input field, it will avoid to type all characters except ```Numeric Characters```   
For more details [http://stackz.ru/en/995183/how-to-allow-only-numeric-0-9-in-html-inputbox-using-jquery](http://stackz.ru/en/995183/how-to-allow-only-numeric-0-9-in-html-inputbox-using-jquery)

### References
@UsamaKhaki
