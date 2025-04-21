## 🔑 **1. `abstract`**

### ✅ **What is it?**

The `abstract` keyword is used to create a class or method **that is incomplete** — it’s meant to be extended or implemented by others.

---

### 🧱 **Abstract Class**

- Cannot be instantiated directly.
- May contain both **abstract** (no body) and **concrete** (with body) methods.

		abstract class Animal {
		    abstract void sound();  // no body
		    void eat() {
		        System.out.println("Eating...");
		    }
		}
		
		class Dog extends Animal {
		    void sound() {
		        System.out.println("Bark");
		    }
		}

### 🧱 **Abstract Method**

- A method with **no body**.
- Must be inside an **abstract class or interface**.

		abstract void run(); // just method declaration

### ✨ Use:

- To define **partial implementation**.
- To force **subclasses to implement** missing parts.

## 🧩 **2. `interface`**

### ✅ **What is it?**

An interface is a **completely abstract class** (in older versions) that contains only **abstract methods** (until Java 8).

Used to define **common behavior** for multiple classes.

	 interface Vehicle {
	    void start();
	}
	
	class Car implements Vehicle {
	    public void start() {
	        System.out.println("Car started");
	    }
	}

### ✅ Java 8+ Enhancements:

Interfaces can now have:

- **default methods** (with body)
- **static methods**

		interface Test {
		    default void show() {
		        System.out.println("Default Method");
		    }
		}

### ✨ Use:

- To achieve **100% abstraction**
- To support **multiple inheritance**
