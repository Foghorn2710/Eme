public class Employee {
 private int id;
 private String name;
 private double salary;
 public Employee(int id, String name, double salary) {
 this.id = id;
 this.name = name;
 this.salary = salary;
 }
 public void raiseSalary(double percent) {
 if (percent > 0) {
 double raise = salary * (percent / 100);
 salary += raise;
 System.out.println(name + "'s salary raised by " + percent + "%. New salary: " + salary);
 } else {
 System.out.println("Please provide a positive percentage for salary raise.");
 }
 }
 public void displayInfo() {
 System.out.println("Employee ID: " + id);
 System.out.println("Name: " + name);
 System.out.println("Salary: " + salary);
 }
 public static void main(String[] args) {
 // Creating an employee object
 Employee emp = new Employee(1001, "John Doe", 50000);
 // Displaying initial information
 System.out.println("Initial Information:");
 emp.displayInfo();
 // Raising salary by a given percentage
 double raisePercentage = 10; // Example: 10% raise
 emp.raiseSalary(raisePercentage);
 // Displaying updated information after the raise
 System.out.println("\nInformation after salary raise:");
 emp.displayInfo();
 }
}
