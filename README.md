class Student {
    private String name;
    private double currentMarks;
    private double percentageIncrease;
    public Student(String name, double currentMarks) {
        this.name = name;
        this.currentMarks = currentMarks;
    }
    public void setPercentageIncrease(double percentage) {
        this.percentageIncrease = percentage;
    }
    public double calculateNewMarks() {
        return currentMarks + (currentMarks * percentageIncrease / 100);
    }
    public void displayDetails() {
        System.out.println("Student Name: " + name);
        System.out.println("Current Marks: " + currentMarks);
        System.out.println("Percentage Increase: " + percentageIncrease + "%");
        System.out.println("New Marks after Percentage Increase: " + calculateNewMarks());
    }
}
public class PercentageIncreaseExample {
    public static void main(String[] args) {
        Student student = new Student("John Doe", 75);
        student.setPercentageIncrease(10);
        student.displayDetails();
    }
}

output
Student Name: John Doe
Current Marks: 75.0
Percentage Increase: 10.0%
New Marks after Percentage Increase: 82.5

