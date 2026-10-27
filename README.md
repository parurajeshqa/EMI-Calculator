EMI Calculator in Java
📌 Project Description

The EMI (Equated Monthly Installment) Calculator is a console-based Java application that calculates the monthly installment for a loan based on the loan amount, annual interest rate, and loan tenure.

The program calculates and displays the monthly EMI, total interest payable, and total payment over the entire loan period. It also handles loans with a zero-interest rate.

✨ Features
Accepts the loan amount from the user.
Accepts the annual interest rate as a percentage.
Accepts the loan tenure in years.
Calculates the monthly interest rate and total number of monthly installments.
Calculates the monthly EMI using a mathematical formula.
Handles zero-interest loans.
Displays the monthly EMI, total interest, and total payment.
Formats financial results to two decimal places.
🛠️ Technologies Used
Programming Language: Java
Input Handling: Scanner class
Mathematical Calculations: Math.pow()
Output Formatting: System.out.printf()
📂 Project Structure
text
EMI-Calculator/
└── src/
    └── day3/
        └── EMICalculator.java

🧮 EMI Calculation Formula

The program uses the standard EMI formula:

𝐸
𝑀
𝐼
=
𝑃
×
𝑅
×
(
1
+
𝑅
)
𝑁
(
1
+
𝑅
)
𝑁
−
1

Where:

P = Principal loan amount
R = Monthly interest rate expressed as a decimal
N = Total number of monthly installments
Supporting Calculations

1. Monthly Interest Rate

java
double monthlyRate = annualRate / (12 * 100);


2. Total Number of Monthly Installments

java
int months = years * 12;


3. Total Payment

java
double totalPayment = emi * months;


4. Total Interest Payable

java
double totalInterest = totalPayment - principal;


If the interest rate is zero, the program calculates the EMI by dividing the principal by the total number of months.

🚀 How to Run the Program
Prerequisites
Java Development Kit (JDK) installed on your computer.
A Java-supported IDE, such as Eclipse, IntelliJ IDEA, or VS Code, or a terminal.
Steps
Clone or download the repository.
Open the project in your preferred Java IDE.
Navigate to EMICalculator.java inside the day3 package.
Run the EMICalculator class.
Enter the loan amount.
Enter the annual interest rate as a percentage.
Enter the loan tenure in years.
View the calculated monthly EMI, total interest, and total payment.
Run Using the Terminal

From the directory containing the day3 folder, execute:

bash
javac day3/EMICalculator.java
java day3.EMICalculator

💻 Example Output

For a loan amount of 100,000, an annual interest rate of 12%, and a loan tenure of 5 years:

text
Enter loan amount: 100000
Enter annual interest rate (%): 12
Enter loan tenure (in years): 5

Monthly EMI: 2224.44
Total Interest: 33466.88
Total Payment: 133466.88


Note: The amounts are shown in generic currency units because the program does not specify a currency.

🎯 Learning Objectives

This project demonstrates the following Java programming concepts:

Accepting user input using the Scanner class.
Using variables and data types such as double and int.
Performing arithmetic operations.
Converting an annual interest rate into a monthly interest rate.
Using Math.pow() for exponentiation.
Implementing conditional logic with if and else.
Formatting decimal output with System.out.printf().
Calculating loan repayment and interest amounts.
Closing input resources with scanner.close().
🔮 Future Improvements
Validate that the loan amount and tenure are positive.
Reject negative interest rates if they are not supported.
Allow users to enter loan tenure in months as well as years.
Support different currencies.
Display a month-by-month loan amortization schedule.
Allow users to compare loans with different interest rates and tenures.
Add a graphical user interface (GUI).
⚠️ Important Notes
The calculator assumes a fixed annual interest rate throughout the loan tenure.
Results are estimates based on the standard EMI formula.
Actual lender calculations may differ due to fees, rounding rules, and other loan terms.
Enter valid positive loan amounts and loan tenures to obtain meaningful results.
👨‍💻 Author

Created as a beginner-level Java project to practice mathematical calculations, conditional statements, user input, and formatted output.

📄 License

This project is intended for educational and learning purposes.
