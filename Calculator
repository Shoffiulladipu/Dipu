#include <stdio.h>
#include <stdlib.h>

int ismarksvalide (int mark)
{
    if (mark>100)
    {
        printf("Invalid Mark please inter mark again\n");

        return ;
    }
    else if (mark<0)
    {
        printf("Invalid Mark please inter mark again\n");

        return ;
    }
    return ;
}
float gettgp(int mark, int credit)
{
    float tgpa;

    if (mark>=80 && mark<=100)
    {
        tgpa = (4.00 * credit);
    }
    else if (mark>=75 && mark<=79)
    {
        tgpa = (3.75 * credit);
    }
    else if (mark>=70 && mark<=74)
    {
        tgpa = (3.50 * credit);
    }
    else if (mark>=65 && mark<=69)
    {
        tgpa = (3.25 * credit);
    }
    else if (mark>=60 && mark<=64)
    {
        tgpa = (3.00 * credit);
    }
    else if (mark>=55 && mark<=59)
    {
        tgpa = (2.75 * credit);
    }
    else if (mark>=50 && mark<=54)
    {
        tgpa = (2.50 * credit);
    }
    else if (mark>=45 && mark<=49)
    {
        tgpa = (2.25 * credit);
    }
    else if (mark>=40 && mark<=44)
    {
        tgpa = (2.00 * credit);
    }
    else
    {
        tgpa = 0;
    }
    return tgpa;
}
float calculategpa (float stgp, int stcredit)
{
    float sgpa;
    sgpa = stgp / stcredit;
    return sgpa;

}
float calculatecgpa (float tgp, float totalcredit)
{
    float cgpa;
    cgpa= tgp/totalcredit;
    return cgpa;
}

int main()
{
    int n,i,j,x,mark,credit,totalcredit=0;
    float tgp,sgpa,tgpa=0,cgpa;
    printf("Total Semesters : ");
    scanf("%d",&n);
    for(i=1; i<=n; i++)
    {
        int stcredit=0;
        float stgp=0;
        printf("\n=====Semester %d======",i);
        printf("\nTotal Subject : ");
        scanf("%d",&x);
        for(j=1; j<=x; j++)
        {
            printf("Subject %d credit : ",j);
            scanf("%d",&credit);
            printf("Subject %d mark :",j);
            scanf("%d",&mark);
            while(ismarksvalide(mark) == 0)
            {
                printf("Enter Subject %d Marks: ", j);
                scanf("%d", &mark);
            }
            stcredit = stcredit + credit;
            totalcredit=totalcredit+credit;
            tgp = gettgp(mark,credit);
            stgp = stgp+tgp;
            tgpa = tgpa + tgp;
            sgpa = calculategpa(stgp,stcredit);
            cgpa = calculatecgpa(tgpa,totalcredit);
        }
        printf("Your Semester GPA is : %.4f\n",sgpa);
        printf("Your CGPA is : %.3f\n",cgpa);
    }
    printf("\n\n\t Design By Shoffiulla Dipu \n Department of CSE In Bangladesh University\n");
    return 0;
}
