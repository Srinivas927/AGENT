# AGENT
import java.util.Scanner;

public class InsuranceManagementSystem {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Sample customers and insurance policies
        Customer customer1 = new Customer("John Doe", "123 Main St", "123-456-7890");
        Customer customer2 = new Customer("Jane Smith", "456 Oak St", "987-654-3210");
        
        Policy policy1 = new Policy("P001", "Health Insurance", 1000.0);
        Policy policy2 = new Policy("P002", "Car Insurance", 1200.0);
        
        customer1.addPolicy(policy1);
        customer2.addPolicy(policy2);

        // Sample Claims
        Claim claim1 = new Claim("C001", policy1, "Health Issue", 500.0);
        Claim claim2 = new Claim("C002", policy2, "Car Accident", 2000.0);
        
        policy1.addClaim(claim1);
        policy2.addClaim(claim2);

        // User Interface to interact with the system
        System.out.println("Welcome to Insurance Management System");
        System.out.println("1. View Customer Details");
        System.out.println("2. View Policy Details");
        System.out.println("3. View Claim Details");
        System.out.println("4. Exit");

        while (true) {
            System.out.print("\nEnter your choice: ");
            int choice = scanner.nextInt();
            scanner.nextLine(); // Consume the
