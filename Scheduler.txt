import java.util.Scanner;
class Exam_scheduler
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter no. of Subjects ");
        int l=sc.nextInt();
        int b;
        String Sub;
        int date;
        String exam[][]=new String[3][7];
        String date1="11-04-2021 (enter 1 for this date)";
        String date2="12-04-2021 (enter 2 for this date)";
        String slot1="slot- 11:30-12:30 (enter 1 for this slot)";
        String slot2="slot- 12:30-13:30 (enter 2 for this slot)";
        String slot3="slot- 13:30-14:30 (enter 3 for this slot)";
        String slot4="slot- 14:30-15:30 (enter 4 for this slot)";
        String slot5="slot- 15:30-16:30 (enter 5 for this slot)";
        String slot6="slot- 16:30-17:30 (enter 6 for this slot)";
        exam[0][0]="date/time";
        exam[1][0]="11-04-2021";
        exam[2][0]="12-04-2021";
        exam[0][1]="11:30-12:30";
        exam[0][2]="12:30-13:30";
        exam[0][3]="13:30-14:30";
        exam[0][4]="14:30-15:30";
        exam[0][5]="15:30-16:30";
        exam[0][6]="16:30-17:30";
        for(int i=0;i<l;i++)
        {
            System.out.println("Enter name of Subject ");
            Sub=sc.next();
            System.out.println("Following are the dates for exam. Please select one...");
            System.out.println(date1);
            System.out.println(date2);
            date=sc.nextInt();
            if(date == 1)
            {
                System.out.println("Following are the time slots for exam. Please select one...");
                System.out.println(slot1);
                System.out.println(slot2);
                System.out.println(slot3);
                System.out.println(slot4);
                System.out.println(slot5);
                System.out.println(slot6);
                b=sc.nextInt();
                if(b==1)
                {
                    if(exam[1][1] == null) 
                    exam[1][1]=Sub;
                    else{
                    System.out.println("Slot not available");
                    }
                }
                if(b==2)
                {
                    if(exam[1][2] == null) 
                    exam[1][2]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==3)
                {
                    if(exam[1][3] == null) 
                    exam[1][3]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==4)
                {
                    if(exam[1][4] == null) 
                    exam[1][4]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==5)
                {
                    if(exam[1][5] == null) 
                    exam[1][5]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==6)
                {
                    if(exam[1][6] == null) 
                    exam[1][6]=Sub;
                    else
                    System.out.println("Slot not available");
                }
            }
            else if(date == 2)
            {
                System.out.println("Following are the time slots for exam. Please select one...");
                System.out.println(slot1);
                System.out.println(slot2);
                System.out.println(slot3);
                System.out.println(slot4);
                System.out.println(slot5);
                System.out.println(slot6);
                b=sc.nextInt();
                if(b==1)
                {
                    if(exam[2][1] == null) 
                    exam[2][1]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==2)
                {
                    if(exam[2][2] == null) 
                    exam[2][2]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==3)
                {
                    if(exam[2][3] == null) 
                    exam[2][3]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==4)
                {
                    if(exam[2][4] == null) 
                    exam[2][4]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==5)
                {
                    if(exam[2][5] == null) 
                    exam[2][5]=Sub;
                    else
                    System.out.println("Slot not available");
                }
                if(b==6)
                {
                    if(exam[2][6] == null) 
                    exam[2][6]=Sub;
                    else
                    System.out.println("Slot not available");
                }
            }
            else
            {
                System.out.println("this date is not assigned for examination, please enter right date");
            }
        }
        System.out.println("Thank you, your exams are succesfully scheduled");
        for(int i=0;i<3;i++)
        {
            for(int j=0;j<7;j++)
            {
                System.out.print("|"+exam[i][j]+" |");
            }
            System.out.println();
        }
    }
}