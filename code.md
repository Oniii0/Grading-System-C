// Grade Average - Grade Marks BY GROUP 5

#include <stdio.h>

int main(void) {
  // Declare variables to store the grades and the student's name
  float grade1, grade2, grade3, grade4, grade5, grade6, grade7, grade8, grade9,
      grade10;
  float average;
  float grade;
  char name[100];

  // Prompt the user to input their name
  system("clear"); // Clear the output
  printf("Enter your name: ");
  scanf("%[^\n]", name);

  // Prompt the user to input their grades
  system("clear"); // Clear the output
  printf("Enter your grade for Computer Programming: ");
  scanf("%f", &grade1);
  system("clear"); // Clear the output
  printf("Enter your grade for Computer System Servicing: ");
  scanf("%f", &grade2);
  system("clear"); // Clear the output
  printf("Enter your grade for ICT (E-TECH): ");
  scanf("%f", &grade3);
  system("clear"); // Clear the output
  printf("Enter your grade for KPWKP: ");
  scanf("%f", &grade4);
  system("clear"); // Clear the output
  printf("Enter your grade for General Mathematics: ");
  scanf("%f", &grade5);
  system("clear"); // Clear the output
  printf("Enter your grade for Personal Development: ");
  scanf("%f", &grade6);
  system("clear"); // Clear the output
  printf("Enter your grade for Physical Education and Health: ");
  scanf("%f", &grade7);
  system("clear"); // Clear the output
  printf("Enter your grade for Oral Communication: ");
  scanf("%f", &grade8);
  system("clear"); // Clear the output
  printf("Enter your grade for Earth and Life Science: ");
  scanf("%f", &grade9);
  system("clear"); // Clear the output
  printf("Enter your grade for Theology: ");
  scanf("%f", &grade10);

  // Calculate the average grade
  average = (grade1 + grade2 + grade3 + grade4 + grade5 + grade6 + grade7 +
             grade8 + grade9 + grade10) /
            10;

  // Display the grades that the user input
  system("clear"); // Clear the output
  printf("-----------------------------------\n");
  printf("            Your grades\n");
  printf("-----------------------------------\n");
  printf("|Computer Programming          :%.0f|\n", grade1);
  printf("|Computer System Servicing     :%.0f|\n", grade2);
  printf("|ICT (E-TECH)                  :%.0f|\n", grade3);
  printf("|KPWK:                         :%.0f|\n", grade4);
  printf("|General Mathematics           :%.0f|\n", grade5);
  printf("|Personal Development          :%.0f|\n", grade6);
  printf("|Physical Education and Health :%.0f|\n", grade7);
  printf("|Oral Communication            :%.0f|\n", grade8);
  printf("|Earth and Life Science        :%.0f|\n", grade9);
  printf("|Theology                      :%.0f|\n", grade10);
  printf("-----------------------------------\n");

  // Output of Average
  printf("%s, Your Average Grade is: %.2f\n", name, average);

  // Determine Grade Marks
  printf("-----------------------------------\n");
  printf("If you wanna know your Grade Mark \nEnter your Average: ");
  scanf("%f", &grade);
  if (grade <= 100 && grade >= 90) {
    printf("-----------------------------------\n");
    printf("You Got Grade A\n");
  } else if (grade < 90 && grade >= 85) {
    printf("-----------------------------------\n");
    printf("You Got Grade B\n");
  } else if (grade < 85 && grade >= 80) {
    printf("-----------------------------------\n");
    printf("You Got Grade C\n");
  } else if (grade < 80 && grade >= 75) {
    printf("-----------------------------------\n");
    printf("You Got Grade D\n");
  } else {
    printf("-----------------------------------\n");
    printf("You Got Grade F\n");
  }
  if (grade < 75) {
    printf("You didn't pass the Semester.\n");
    printf("-----------------------------------\n");
  } else {
    printf("You passed the Semester.\n");
    printf("-----------------------------------\n");
  }
  printf("Thanks for using the Grading System!\n");
  printf("-----------------------------------\n");
  return 0;
}
