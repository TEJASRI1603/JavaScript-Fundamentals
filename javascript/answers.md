✅ let — Answers
Q1
let x = 10;
x = 20;
console.log(x);


✅ Answer: 20
Because let can be updated, just not redeclared.

Q2
let a = 5;
let a = 6;
console.log(a);


❌ Error: Identifier 'a' has already been declared
Because let cannot be redeclared in the same scope.

Q3
{
  let y = 50;
  console.log(y);
}
console.log(y);


First log → 50
Second log → ❌ Error: y is not defined

Because let is block scoped, available only inside { }.

✅ const — Answers
Q1
const city = "Delhi";
city = "Mumbai";


❌ Error: Assignment to constant variable.
const cannot be reassigned.

Q2
const numbers = [1, 2];
numbers.push(3);
console.log(numbers);


✅ Answer: [1, 2, 3]

const prevents reassignment, but modifying array/object content is allowed.

Q3
const obj = { x: 10 };
obj.x = 20;
console.log(obj.x);


✅ Answer: 20
Same reason — object properties can be changed in const objects.

✅ var — Answers
Q1
var a = 10;
var a = 20;
console.log(a);


✅ Answer: 20
Because var allows redeclaration.

Q2
if (true) {
  var name = "Ram";
}
console.log(name);


✅ Answer: "Ram"

var is function scoped, not block scoped, so it leaks outside the if.

Q3
console.log(z);
var z = 30;


✅ Answer: undefined

Because var is hoisted, but only its declaration moves up, not the value.