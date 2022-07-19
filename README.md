1a ANONYMOUS FUNCTION

var oddfn = function(array) {
  for(var i=0;i<array.length;i++){
  if (array == null){ 
    return void 0;
  }
  if(array[i]%2!=0){
    console.log(array[i]);
  }else{
    continue;
  }
  }
};

console.log(oddfn([5, 4, 3, -2]));

1b ANONYMOUS FUNCTION

var upper = function(array) {
  for(var i=0;i<array.length;i++){
    if(array[i]==array[i].toLowerCase()){
      array[i] = array[i].toUpperCase();
    }
  }
  return array;
};

console.log(upper(["string","lols","abs","dead"]));

1c ANONYMOUS FUNCTION

var add = function(array,sum) {
  sum = 0;
  for(var i=0;i<array.length;i++){
    sum = sum + array[i]
  }
  return sum;
};

console.log(add([4,10,6,7]));

1d ANONYMOUS FUNCTION

var isPrime = function(array,array2) {
  array2 = [];
  for(var i=0;i<array.length;i++){
    for(var j=2;j<array[i]/2;j++){
      if(array[i]%j!=0){
        array2 += array[i]+" ";
        break;
      }else if(array[i]%j==0){
        break;
      }
    }
  }
  return array2;
};

console.log(isPrime([4,6,7,23]));

1e ANONYMOUS FUNCTION

var isPalindrome = function(array,array2) {
  array2 = "";
  for(var i=0;i<array.length;i++){
    len = Math.floor(array[i].length);
    string = array[i];
    rev = string.split('').reverse().join('');
    if(string==rev){
      array2 += rev + " ";
    }else{
      break;
    }
  }
  return array2;
};

console.log(isPalindrome(["mom","lool",'xdx',"sdsd"]));

1f ANONYMOUS FUNCTION

var median = function(array,array2) {
  if(array.length==array2.length){
    for(let i=0;i<array2.length;i++){
      array3 = [...array,...array2];
      sum = 0;
      for(let i=0;i<array3.length;i++){
        len = array3.length;
        sum += array3[i];
        avg = sum/len;
      }
    }
  }
  return avg;
};

console.log(median([4,10,5,15],[12,5,8,8]));

1g ANONYMOUS FUNCTION

var dup = function(array) {
  return Array.from(new Set(a));
};

console.log(dup([4,10,5,4,15]));

1h ANONYMOUS FUNCTION

var rshift = function(array,n) {
  for(let i=0;i<n;i++){
    array.unshift(array.pop());
  }
  return array;
};

console.log(rshift([4,10,5,4,23],4));

1a IIFE FUNCTION

function(oddfn(array)) {
  for(var i=0;i<array.length;i++){
  if (array == null){ 
    return void 0;
  }
  if(array[i]%2!=0){
    console.log(array[i]);
  }else{
    continue;
  }
  }
};

console.log(oddfn([5, 4, 3, -2]));

1b IIFE FUNCTION

function(upper(array)) {
  for(var i=0;i<array.length;i++){
    if(array[i]==array[i].toLowerCase()){
      array[i] = array[i].toUpperCase();
    }
  }
  console.log(array);
};

console.log(upper(["string","lols","abs","dead"]));

1c IIFE FUNCTION

function(add(array,sum)) {
  sum = 0;
  for(var i=0;i<array.length;i++){
    sum = sum + array[i]
  }
  console.log(sum);
};

console.log(add([4,10,6,7]));

1d IIFE FUNCTION

function(array,array2) {
  array2 = [];
  for(var i=0;i<array.length;i++){
    for(var j=2;j<array[i]/2;j++){
      if(array[i]%j!=0){
        array2 += array[i]+" ";
        break;
      }else if(array[i]%j==0){
        break;
      }
    }
  }
  console.log(array2);
};

console.log(isPrime([4,6,7,23]));

1e IIFE FUNCTION

function(isPalindrome(array,array2)) {
  array2 = "";
  for(var i=0;i<array.length;i++){
    len = Math.floor(array[i].length);
    string = array[i];
    rev = string.split('').reverse().join('');
    if(string==rev){
      array2 += rev + " ";
    }else{
      break;
    }
  }
  console.log(array2);
};

console.log(isPalindrome(["mom","lool",'xdx',"sdsd"]));

1f IIFE FUNCTION

var median = function(array,array2) {
  if(array.length==array2.length){
    for(let i=0;i<array2.length;i++){
      array3 = [...array,...array2];
      sum = 0;
      for(let i=0;i<array3.length;i++){
        len = array3.length;
        sum += array3[i];
        avg = sum/len;
      }
    }
  }
  console.log(avg);
};

console.log(median([4,10,5,15],[12,5,8,8]));

1g IIFE FUNCTION

function(dup(array)) {
  console.log(Array.from(new Set(a)));
};

console.log(dup([4,10,5,4,15]));

1h IIFE FUNCTION

function(rshift(array,n)) {
  for(let i=0;i<n;i++){
    array.unshift(array.pop());
  }
  console.log(array);
};


2a ARROW FUNCTION

var oddfn = (array) => {
  for(var i=0;i<array.length;i++){
  if (array == null){ 
    return void 0;
  }
  if(array[i]%2!=0){
    console.log(array[i]);
  }else{
    continue;
  }
  }
};

console.log(oddfn([5, 4, 3, -2]));

2b ARROW FUNCTION

var upper = (array) => {
  for(var i=0;i<array.length;i++){
    if(array[i]==array[i].toLowerCase()){
      array[i] = array[i].toUpperCase();
    }
  }
  return array;
};

console.log(upper(["string","lols","abs","dead"]));

2c ARROW FUNCTION

var add = (array,sum) => {
  sum = 0;
  for(var i=0;i<array.length;i++){
    sum = sum + array[i]
  }
  return sum;
};

console.log(add([4,10,6,7]));

2d ARROW FUNCTION

var isPrime = (array,array2) => {
  array2 = [];
  for(var i=0;i<array.length;i++){
    for(var j=2;j<array[i]/2;j++){
      if(array[i]%j!=0){
        array2 += array[i]+" ";
        break;
      }else if(array[i]%j==0){
        break;
      }
    }
  }
  return array2;
};

console.log(isPrime([4,6,7,23]));

2e ARROW FUNCTION

var isPalindrome = (array,array2) => {
  array2 = "";
  for(var i=0;i<array.length;i++){
    len = Math.floor(array[i].length);
    string = array[i];
    rev = string.split('').reverse().join('');
    if(string==rev){
      array2 += rev + " ";
    }else{
      break;
    }
  }
  return array2;
};

console.log(isPalindrome(["mom","lool",'xdx',"sdsd"]));
