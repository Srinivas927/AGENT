# AGENT
class Policy {
    private String policyNumber;
    private String policyType;
    private double coverageAmount;
    private Customer customer;

    // Constructor
    public Policy(String policyNumber, String policyType, double coverageAmount, Customer customer) {
        this.policyNumber = policyNumber;
        this.policyType = policyType;
        this.coverageAmount = coverageAmount;
        this.customer = customer;
    }

    // Getters and Setters
    public String getPolicyNumber() {
        return policyNumber;
    }

    public String getPolicyType() {
        return policyType;
    }

    public double getCoverageAmount() {
        return coverageAmount;
    }

    public Customer getCustomer() {
        return customer;
    }

    @Override
    public String toString() {
        return "Policy{policyNumber='" + policyNumber + "', policyType='" + policyType + "', coverageAmount=" + coverageAmount + ", customer=" + customer.getName() + "}";
    }
}
