🔹 What is an Object?

An object in JavaScript is a collection of key–value pairs.
It is used to store multiple pieces of information inside one structure.

Example:

const person = {
  name: "Ram",
  age: 21,
  city: "Hyderabad"
};

🔹 Why Do We Use Objects?

To store structured data

To group related values

To represent real-world things (user, product, order, car, etc.)

🔹 Accessing Object Values
1. Dot notation:
console.log(person.name);

2. Bracket notation:
console.log(person["city"]);

🔹 Adding New Properties
person.job = "Developer";

🔹 Updating Properties
person.age = 22;

🔹 Deleting Properties
delete person.city;

🔹 Nested Objects
const user = {
  name: "Ram",
  address: {
    city: "Hyderabad",
    pin: 500001
  }
};

console.log(user.address.city);

🔹 Array of Objects
const students = [
  { name: "Ram", age: 21 },
  { name: "Sam", age: 22 }
];

console.log(students[0].name);

🔹 Methods Inside Objects
const car = {
  brand: "Tesla",
  run() {
    console.log("Car is running");
  }
};

car.run();

📝 6 Practice Questions

Create an object called book with title, author, and price.

Update the price of the book.

Add a new property pages to the book.

Delete the author property.

Create a nested object profile with username, and details containing age and city.

Print profile.details.age.