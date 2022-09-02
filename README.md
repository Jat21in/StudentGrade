# StudentGrade
#include <stdio.h>
int main() {
    printf("****************** Welcome To Program To Display Student Grade *************************");
    char studentname ,studentclass, studentgrade ;
    int rollno , m1 , m2 , m3 , m4 , m5 ;
    double totalmarks , percentagemarks ;\

    printf("Enter Student's Name :");
    scanf("%c /n",&studentname);

    printf("Enter Class :");
    scanf("%c /n",&studentclass);

    printf("Enter Marks in 5 Subjects :");
    scanf("%d /n",& m1);
    scanf("%d /n",& m2);
    scanf("%d /n",& m3);
    scanf("%d /n",& m4);
    scanf("%d /n",& m5);

    totalmarks = m1+m2+m3+m4+m5 ;

    percentagemarks = (totalmarks/500.0)*100;

    if(percentagemarks >= 95 )
       studentgrade= "A+";
    else if ((percentagemarks >=85 ) && (percentagemarks < 95))
       studentgrade = "A" ;
    else if ((percentagemarks >=75 ) && (percentagemarks < 85))
       studentgrade = "B" ;
    else if ((percentagemarks >=55 ) && (percentagemarks < 75))
       studentgrade = "C" ;
    else if ((percentagemarks >=40 ) && (percentagemarks < 55))
       studentgrade = "D" ;
    else 
        studentgrade = "E" ;

    printf("Student's Name is : %c",studentname);
    printf("Class: %c",studentclass);
    printf("Roll Number : is : %d",rollno);
    printf("Marks : %d",m1,m2,m3,m4,m5);
    printf("Total Marks : %d",totalmarks);
    printf("Percentage Marks : %d", percentagemarks);
    printf("Grade : %c", studentgrade);

    return 0;
}

