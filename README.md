# Drumkit-Game
Objects, Methods &amp; Dot Notation in JavaScript Objects hold properties (data) and methods (functions).  Properties are accessed with object.property.  Methods are called with object.method().  Constructor functions act as blueprints to create multiple objects with shared properties and methods.
# 🟡 Objects, Methods & Dot Notation in JavaScript

## 📌 Overview
In JavaScript, **objects** are containers for data (**properties**) and actions (**methods**).  
- **Property** → `object.property`  
- **Method** → `object.method()`  

Methods are simply **functions attached to objects**.  
Dot notation makes it easy to access both.

---

## 🚀 Example: HouseKeeper Constructor

```javascript
// Constructor Function (Blueprint)
function HouseKeeper(name, exp, area) {
  this.name = name;
  this.experience = exp;
  this.cleaningArea = area;
  
  // Method
  this.clean = function() {
    alert("Cleaning in progress...");
  };
}

// Create an object
const houseKeeper1 = new HouseKeeper("James", 12, "bedrooms");

// Call method
houseKeeper1.clean(); // "Cleaning in progress..."

