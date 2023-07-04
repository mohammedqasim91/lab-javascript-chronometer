good job, but you have some mistakes that makes the code not able to work, luckily they can be solved quickly:)

in index.js you should call for 'chronometer.split()' instead of calling 'chronometer.splitClick()', because the last one doesn't exist in chronometer.js
in chronometer.js you should modify the function in line 28 to look like this:

  computeTwoDigitsNumber(number) {
    return number < 10 ? `0${number}` : `${number}`;
  }

because you were using 'number' but the argument was called 'value' so 'number' didn't exist
and be careful with the name of the function, because it was being called from index.js but with another name 'digits' was singular 
