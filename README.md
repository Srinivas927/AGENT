# AGENT
class Customer {
    private String name;
    private int age;
    private String address;
    private String phoneNumber;

    // Constructor
    public Customer(String name, int age, String address, String phoneNumber) {
        this.name = name;
        this.age = age;
        this.address = address;
        this.phoneNumber = phoneNumber;
    }

    // Getters and Setters
    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    public String getAddress() {
        return address;
    }

    public String getPhoneNumber() {
        return phoneNumber;
    }

    @Override
    public String toString() {
        return "Customer{name='" + name + "', age=" + age + ", address='" + address + "', phoneNumber='" + phoneNumber + "'}";
    }
}
