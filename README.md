# Difference-Objects-Classes-
// CLASS - Blueprint (defines structure)
class Car {
    String name;  // All cars have names, but specific name is unknown

    // Constructor - initializes data when object is created
    public Car(String carName) {
        name = carName;  // Sets specific name for concrete object
    }

    // Method - all cars have a unique brand&model
    public void model() {
        System.out.println("My car is a" + name +".");
    }
}

// Main class - demonstrates object creation
public class Demo {
    public static void main(String[] args) {
        // Create OBJECTS - concrete instances from blueprint
        Car mycar1 = new Car("Ford-150");     // First object
        Car mycar2 = new Car("Tesla-Cybertruck");   // Second object

        // Each object has its own data
        mycar1.model();  // Output: My car is a Ford-150.
        mycar2.model();  // Output: My car is a Tesla-Cybertruck.

        // Prove they are different objects
        System.out.println("Are they same? " + (mycar1 == mycar2)); // Output: false
    }
}
