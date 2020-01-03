# solved-tasks
* task 1
```javascript
const a = 123;
const b = 456;
// test
// Hello world!
const arr = [];
let arr2 = [];
```
*task 2
```javascript
function greet() {
  let str = 'hello world!';
  
  return str;
}
```
*task 3
```javascript
function helloWorld() {
  var str = 'Hello World!';
  console.log(str);
  return str;
}//refer to the example and write your first JS function
```
*task 4
```javascript
const howMuchILoveYou = n => ['I love you', 'a little', 'a lot', 'passionately', 'madly', 'not at all'];
```
*task 5
```javascript
function iceBrickVolume(radius,bottleLength,rimLength){
return 2*radius**2(bottleLength - rimLength);
}
```
*task 6
```javascript
function past(h, m, s){
return h * 3600000 + m * 60000 + s * 1000
}
```
*task 7
```javascript
function otherAngel($a, $b){
return 180 - $a - $b;
}
```
*task 8
```javascript
const angle = n => (n - 2) * 180; 
```
*task 9
```javascript
function ifChackSaySo(){return !true;}
```
*task 10
```javascript
function boolToWord(){
if(bool === true){
return 'Yes';
}else{
return'No';
}
}
```
*task 11
```javascript
function typeOfSum(a, b){
return typeof(a + b);
}
```
*task 12
 ```javascript
function problem(x){

if (typeof x=='number') {

return (x*50)+6;
} else {
return "Error";
}
}
```
*task 13
```javascript
function numberToString(num) {
  return String(num);
}
```
*task 14
```javascript
const stringToNumber = str => +str;
```
*task 15
```javascript
function sumStr(a,b) {
  return (+a+ +b) + ''
}
```
* task 16
```javascript
const booleanToString = b => `${b}`
```
* task 17
```javascript
function squares(x, n) {
  let arr = [];
  for (let i = 0; i < n; ++i) {
    arr.push(x)
    x = Math.pow(x, 2)
  }
  return arr;
}
```
*task 18
```javascript
const squareOrSquareRoot = array => 
  array.map(el => Number.isInteger(Math.sqrt(el))
    ? Math.sqrt(el)
    : el**2
 );   


```
*task 19
```javascript
const squareDigits = num =>
  Number(
    String(num)
      .split('')
      .map(digit => digit ** 2)
      .join('')
  )
```
*task 20
```javascript
const elevator = (left, right, call) => Math.abs(call - left) < Math.abs(call - right) ? 'left' : 'right'
```
*task 21
```javascript
const sixToast = num => Math.abs(num - 6) 
```
*task 22
```javascript
const findChildren = (santasList, children) => [...new Set(children.filter(name => santasList.includes(name)).sort())]
```
*task 23
```javascript
const countWins = (winnerList, countryToCompare) =>
  winnerList.reduce((total, { country }) => (country === countryToCompare ? total + 1 : total), 0)
```
*task 24
```javascript
function well(x) {
  const count = x.reduce((s, v) => s + (v == 'good'), 0);
  return count ? count > 2 ? 'I smell a series!' : 'Publish!' : 'Fail!';
}
```
*task 25
```javascript
const removeEveryOther = arr => arr.filter((_, i) => i % 2 === 0);
```
*task 26
```javascript
function filterEvenLengthWords(words) {
  var evenLengths = []
  for (var i = 0; i < words.length; ++i) {
    if (words[i].length % 2 === 0) {
      evenLengths.push(words[i]);
    }
  }
  return evenLengths
}
```
*task 27
```javascript
function isPalindrome(x) {
  x=x.toLowerCase()
  return x===x.split``.reverse().join``
}
```
* task 28
```javascript
function solution(str){
  return str.split('').reverse().join('');  
}
```
* task 29
```javascript
var uniqueInOrder = function(iterable) {
  if (typeof iterable === "string")
    return iterable.split("").filter((v, i, arr) => arr[i] != arr[i + 1]);
  return iterable.filter((v, i, arr) => arr[i] != arr[i + 1]);
};
```
* task 30
```javascript
const spacify = str => [...str].join(' ')
```
* task 31
```javascript
function digits(z){
let num = z
    .toString()
    .split("")
    .map(v => v * 1);
  let arr = [];
  for (let i = 0; i < num.length; i++) {
    for (let j = 1 + i; j < num.length; j++) {
      arr.push(num[i] + num[j]);
    }
  }
  return arr;
}
```
* task 32
```javascript
function determineTime(durations){
  let hours = 0;
  let min = 0;
  let sec = 0;
  durations.map(v =>
    v
      .split(":")
      .map((v, i) =>
        i === 0 ? (hours += v * 1) : i === 1 ? (min += v * 1) : (sec += v * 1)
      )
  );
  min += sec / 60;
  hours += min / 60;
  return hours <= 24;
}
```
* task 33
```javascript
function stringToArray(string){

	return string.split(' ');
}
```
* task 34
```javascript
function reverse(string) {
  return string
    .split(" ")
    .reverse()
    .join(" ");
}
```
* task 35
```javascript
function type(value) {
  if (value instanceof Array) return 'array'
  if (value instanceof Date) return 'date'
  if (value === null) return 'null'
  if (value instanceof Object) return 'object'
  return typeof value
}
```
* task 36
```javascript
const database = {
  english: 'Welcome',
  czech: 'Vitejte',
  danish: 'Velkomst',
  dutch: 'Welkom',
  estonian: 'Tere tulemast',
  finnish: 'Tervetuloa',
  flemish: 'Welgekomen',
  french: 'Bienvenue',
  german: 'Willkommen',
  irish: 'Failte',
  italian: 'Benvenuto',
  latvian: 'Gaidits',
  lithuanian: 'Laukiamas',
  polish: 'Witamy',
  spanish: 'Bienvenido',
  swedish: 'Valkommen',
  welsh: 'Croeso',
}

const greet = language => database[language] || database.english

```
* task 37
```javascript
const duckDuckGoose = (players, goose) =>
  players[(goose - 1) % players.length].name
```
* task 38
```javascript
let pairs = { A: "T", T: "A", C: "G", G: "C" };
const DNAStrand = dna => dna.replace(/./g, c => pairs[c]);
```
* task 39
```javascript
function maskify(cc) {
return cc.slice(0,-4).replace(/\w/g,'#')+cc.slice(-4)
}
```
* task 40
```javascript
function match({minSalary}, {maxSalary}) {
if (!minSalary || !maxSalary) throw new Error('')
return minSalary*0.9<=maxSalary
}
```
* task 41
```javascript
questions.forEach(function(q) {
  q.usersAnswer = null;
});
```
* task 42
```javascript
function countLanguages(list) {
  const obj = {};
  list.map(v => (obj[v.language] = (obj[v.language] || 0) + 1));
  return obj;
}
```
* task 43
```javascript
function numObj(s) {
  const arr = [];
  s.map(v => arr.push(String.fromCharCode(v)));
  const obj = Array.from({ length: s.length }, x => (x = {}));
  obj.map((v, i) => (v[s[i]] = arr[i]));
  return obj;
}
```
* task 44
```javascript
function arithmetic(a, b, operator){
  var obj = {add: (a + b), subtract: (a-b), multiply: (a * b), divide: (a/b)}
  
  return obj[operator];
}
```
* task 45
```javascript
function accum(s) {
  return s
    .split("")
    .map((c, i) => c.toUpperCase() + c.toLowerCase().repeat(i))
    .join("-");
}
```
 * task 46
 ```javascript
function testit(s){
      if (s.length === 0) return s;
      let sArr = s.split(" ");
      for (let i = 0; i < sArr.length; i++) {
            let as = sArr[i];
            if (as.length > 1) {
                sArr[i] = as.substring(0, as.length - 1) + as.substring(as.length - 1).toUpperCase();
            } else {
                sArr[i] = as.toUpperCase();
            }
        }
        return sArr.join(" ");
}
``` 
* task 47
```javascript
const dontGiveMeFive = (start, end) =>
  Array
    .from(Array(end - start + 1), (_, i) => i + start)
    .filter(num => !num.toString().includes('5'))
    .length
```
* task 48
```javascript
function spEng(s){
return /english/i.test(s)
}
```
* task 49
```javascript
function repeatStr (n, s) {
  return s.repeat(n);
}
```