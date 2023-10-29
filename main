#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
#include<windows.h>
#include<string.h>
#include<time.h>

struct student
{
    char name[100];
    char fname[100];
    char mname[100];
    char phone[20];
    char fphone[20];
    char mphone[20];
    char email[100];
    char address[100];
    char dept[100];
    long long id;
    char dob[100];
    char gender[10];
    char date[100];
    double cgpa;
} std;


COORD coord = {0, 0};

int main()
{
    //system("color f1");
    int key;
    gotoxy(43, 5);
    printf(" WELCOME TO TM UNIVERSITY ");
    gotoxy(50, 8);
    printf("OPTIONS");
    gotoxy(46, 10);
    printf("[1] . LOGIN ");
    gotoxy(46, 11);
    printf("[2] . USER GUIDLINE ");
    gotoxy(46, 12);
    printf("[3] . ABOUT ME");
    gotoxy(46, 13);
    printf("[4] . EXIT");
    gotoxy(40, 16);
    printf("Please Enter Your Choice [1-4] : ");
    scanf("%d", &key);
    if (key != 1 && key != 2 && key != 3 && key!=4)
    {
        system("cls");
        main();
    }
    if(key==1)
        loginAdmin();
    else if(key==2)
        loginTeacher();
    else if(key==3)
        main();
    else if(key==4)
        exit(0);

}

void gotoxy(int a, int b)
{
    coord.X = a;
    coord.Y = b;
    SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE), coord);
}

void loginPage()
{
    system("CLS");
    int key;
    gotoxy(43, 5);
    printf(" WELCOME TO TM UNIVERSITY ");
    gotoxy(48, 8);
    printf("ACCOUNT TYPE");
    gotoxy(46, 10);
    printf("[1] . ADMIN ");
    gotoxy(46, 11);
    printf("[2] . TEACHER ");
    gotoxy(46, 13);
    printf("[3] . RETURN HOME");
    gotoxy(46, 14);
    printf("[4] . EXIT");
    gotoxy(40, 16);
    printf("Please Enter Your Choice [1-4] : ");
    scanf("%d", &key);
    if (key != 1 && key != 2 && key != 3 && key!=4)
    {
        system("cls");
        main();
    }
    if(key==1)
        loginAdmin();
    else if(key==2)
        loginTeacher();
    else if(key==3)
    {
        system("CLS");
        main();
    }

    else if(key==4)
        exit(1);
}

void teacherMenu()
{

    system("CLS");
    gotoxy(47, 5);
    printf("WELCOME TO TEACHER MENU");
    gotoxy(44, 7);
    printf("===========================");
    gotoxy(44, 8);
    printf("[1] . Grade Submission");
    gotoxy(44, 9);
    printf("[2] . Exam Marks Submission");
    gotoxy(44, 10);
    printf("[3] . View Student Details");
    gotoxy(44, 11);
    printf("[4] . Talk To Parents");
    gotoxy(44, 12);
    printf("[5] . Attendance Management");
    gotoxy(44, 13);
    printf("[6] . Log Out!");
    gotoxy(44, 14);
    printf("============================");
    gotoxy(42, 16);
    printf("Please Enter Your Choice [1-6] : ");
    teacherChoice();
}

void adminMenu()
{
    system("CLS");
    gotoxy(47, 5);
    printf("WELCOME TO ADMIN MENU");
    gotoxy(44, 7);
    printf("===========================");
    gotoxy(44, 8);
    printf("[1] . Enroll A Student");
    gotoxy(44, 9);
    printf("[2] . View All Students List");
    gotoxy(44, 10);
    printf("[3] . View Student Details");
    gotoxy(44, 11);
    printf("[4] . Modify Student Record");
    gotoxy(44, 12);
    printf("[5] . Delete Student Record");
    gotoxy(44, 13);
    printf("[6] . Delete All Students");
    gotoxy(44, 14);
    printf("[7] . Log Out!");
    gotoxy(44, 15);
    printf("============================");
    gotoxy(42, 17);
    printf("Please Enter Your Choice [1-7] : ");
    adminChoice();
}

void loginAdmin()
{
    system("cls");
    char user[100];
    char pass[100];
    gotoxy(50, 8);
    printf("ADMIN LOGIN");
    gotoxy(44, 10);
    printf("Enter Your Username    : ");
    scanf(" %[^\n]", user);
    gotoxy(45, 12);
    printf("Enter Password         : ");
    scanf(" %[^\n]", pass);

    if ((strcmp(user, "admin") == 0 && strcmp(pass, "tm") == 0))
    {
        gotoxy(38, 16);
        printf("You Have Successfully Logged In As An Admin");
        gotoxy(44, 20);
        printf("Press [Enter] To Continue -> ");
        int key = getch();
        if (key == 13)
        {
            adminMenu();
        }
        else
            main();
    }
    else
    {
        gotoxy(44, 15);
        printf("Incorrect Login Credentials!");
        gotoxy(44, 17);
        printf("[1] . Try Again");
        gotoxy(44, 18);
        printf("[2] . Return Home");
        gotoxy(44, 19);
        printf("[2] . Exit\n");
        gotoxy(44, 21);
        printf("Please Enter Your Choice [1-3] : ");
        int key;
        scanf("%d", &key);
        if (key == 1)
        {
            system("CLS");
            loginAdmin();
        }

        else if (key == 2)
        {
            system("CLS");
            main();
        }
        else if(key==3)
        {
            exit(1);
        }
    }
}

void loginTeacher()
{
    system("cls");
    char user[100];
    char pass[100];
    gotoxy(50, 8);
    printf("TEACHER LOGIN");
    gotoxy(44, 10);
    printf("Enter Your Username    : ");
    scanf(" %[^\n]", user);
    gotoxy(45, 12);
    printf("Enter Password         : ");
    scanf(" %[^\n]", pass);

    if ((strcmp(user, "teacher") == 0 && strcmp(pass, "tm") == 0))
    {
        gotoxy(38, 16);
        printf("You Have Successfully Logged In As A Teacher");
        gotoxy(44, 20);
        printf("Press [Enter] To Continue -> ");
        int key = getch();
        if (key == 13)
        {
            teacherMenu();
        }
        else
            main();
    }
    else
    {
        gotoxy(44, 15);
        printf("Incorrect Login Credentials!");
        gotoxy(44, 17);
        printf("[1] . Try Again");
        gotoxy(44, 18);
        printf("[2] . Return Home");
        gotoxy(44, 19);
        printf("[2] . Exit\n");
        gotoxy(44, 21);
        printf("Please Enter Your Choice [1-3] : ");
        int key;
        scanf("%d", &key);
        if (key == 1)
        {
            system("CLS");
            loginTeacher();
        }

        else if (key == 2)
        {
            system("CLS");
            main();
        }
        else if(key==3)
        {
            exit(1);
        }
    }
}

void adminChoice()
{
    int key;
    scanf("%d", &key);
    system("cls");
    switch (key)
    {
    case 1:
        std_enroll();
        break;
    case 2:
        std_list();
        break;
    case 3:
        std_detail();
        break;
    case 4:
        std_modify();
        break;
    case 5:
        std_delete();
    case 6:
        deleteAll();
        break;
    case 7:
        main();
        break;
    default:
        adminMenu();
    }
}

void teacherChoice()
{
    int key;
    scanf("%d", &key);
    system("cls");
    switch (key)
    {
    case 1:
        //grade_submit();
        break;
    case 2:
        //marks_submit();
        break;
    case 3:
        //std_det());
        break;
    case 4:
        talk_parents();
        break;
    case 5:
        //attendance();
        break;
    case 6:
        main();
        break;
    default:
        teacherMenu();
    }
}

void std_enroll()
{
    system("CLS");
    FILE *fp;
    fp = fopen("record.txt", "ab+");

    gotoxy(24, 4);
    printf("\t\t\tSTUDENT ENROLLMENT");
    gotoxy(24, 8);
    printf("\t\t\tSTUDENT INFORMATION");
    gotoxy(36, 10);
    printf("[1] . Enter Student's Name           : ");
    scanf(" %[^\n]", std.name);
    gotoxy(36, 11);
    printf("[2] . Enter Student's Gender         : ");
    scanf(" %[^\n]", std.gender);
    gotoxy(36, 12);
    printf("[3] . Enter Student's Date Of Birth  : ");
    scanf(" %[^\n]", std.dob);
    gotoxy(36, 13);
    printf("[4] . Enter Student's Phone Number   : ");
    scanf(" %[^\n]", std.phone);
    gotoxy(36, 14);
    printf("[5] . Enter Student's E-mail         : ");
    scanf(" %[^\n]", std.email);
    gotoxy(36, 15);
    printf("[6] . Enter Student's Address        : ");
    scanf(" %[^\n]", std.address);
    gotoxy(36, 16);
    printf("[7] . Enter Student's Department     : ");
    scanf(" %[^\n]", std.dept);
    gotoxy(36, 17);
    printf("[8] . Set An ID For Student          : ");
    scanf(" %lld", &std.id);
    time_t currentTime;
    time(&currentTime);
    strcpy(std.date, ctime(&currentTime));

    gotoxy(24, 20);
    printf("\t\t\tGUARDIUAN INFORMATION");

    gotoxy(36, 22);
    printf("[1] . Enter Student's Father's Name  : ");
    scanf(" %[^\n]", std.fname);
    gotoxy(36, 23);
    printf("[2] . Enter Father's Phone Number    : ");
    scanf(" %[^\n]", std.fphone);
    gotoxy(36, 24);
    printf("[3] . Enter Student's Mother's Name  : ");
    scanf(" %[^\n]", std.mname);
    gotoxy(36, 25);
    printf("[4] . Enter Mother's Phone Number    : ");
    scanf(" %[^\n]", std.mphone);

    fwrite(&std, sizeof(std), 1, fp);
    fclose(fp);


    gotoxy(38, 27);
    printf("STUDENT HAS BEEN ENROLLED SUCCESSFULLY");
    gotoxy(34, 29);
    printf("Press [ENTER] To Return Home");

    int key = getch();
    if (key == 13)
    {
        adminMenu();
    }

}

void std_detail()
{
    FILE *fp;
    long long idn;
    gotoxy(44, 2);
    printf(" SEARCH STUDENT DETAILS ");
    gotoxy(41, 4);
    printf("Enter Student's ID To Search : ");
    scanf("%lld", &idn);
    if (check(idn) == 1)
    {
        fp = fopen("record.txt", "rb");
        while (fread(&std, sizeof(std), 1, fp))
        {
            if (std.id == idn)
            {
                gotoxy(47, 7);
                printf(" STUDENT DETAILS");
                gotoxy(45, 9);
                printf(" STUDENT INFORMATION");
                gotoxy(36, 11);
                printf("[1] . Name                   : %s", std.name);
                gotoxy(36, 12);
                printf("[2] . ID                     : %lld", std.id);
                gotoxy(36, 13);
                printf("[3] . Department             : %s", std.dept);
                gotoxy(36, 14);
                printf("[4] . CGPA                   : %.2lf", std.cgpa);
                gotoxy(36, 15);
                printf("[5] . Phone Number           : %s", std.phone);
                gotoxy(36, 16);
                printf("[6] . E-mail                 : %s", std.email);
                gotoxy(36, 17);
                printf("[5] . Address                : %s", std.address);
                gotoxy(36, 18);
                printf("[6] . Date Of Admission      : %s", std.date);


                gotoxy(49, 20);
                printf(" PARENTS INFORMATION");
                gotoxy(36, 22);
                printf("[1] . Father's Name          : %s", std.fname);
                gotoxy(36, 23);
                printf("[2] . Mother's Name          : %s", std.mname);
                gotoxy(36, 24);
                printf("[3] . Father's Phone Number  : %s", std.phone);
                gotoxy(36, 25);
                printf("[4] . Mother's Phone Number  : %s", std.phone);
            }
        }
        fclose(fp);
    }
    if (check(idn) == 0)
    {
        system("CLS");
        gotoxy(43, 7);
        printf("NO STUDENT FOUND!!!");
        gotoxy(36, 9);
        printf("[1] . Try Again");
        gotoxy(36, 10);
        printf("[2] . Return To Menu");
        gotoxy(36, 11);
        printf("[3] . Exit\n");
        gotoxy(36, 13);
        printf("Please Enter Your Choice [1-3] : ");
        int key;
        scanf("%d", &key);
        if (key == 1)
        {
            system("CLS");
            std_detail();
        }
        else if (key == 2)
        {
            system("CLS");
            adminMenu();
        }

        else if (key == 3)
        {
            exit(1);
        }
    }
    gotoxy(40, 27);
    printf("Press [ENTER] To Return Home");

    int key = getch();
    if (key == 13)
    {
        system("CLS");
        adminMenu();
    }
    else
    {
        system("CLS");
        std_detail();
    }

}

void std_modify()
{
    FILE *fp, *temp;
    long long idn;

    gotoxy(51, 2);
    printf(" EDIT STUDENT RECORD ");
    gotoxy(42, 4);
    printf("Enter Student ID To Modify : ");
    scanf("%lld", &idn);
    if (check(idn) == 1)
    {
        fp = fopen("record.txt", "rb");
        temp = fopen("temp.txt", "wb");
        while (fread(&std, sizeof(std), 1, fp))
        {
            if (std.id != idn)
                fwrite(&std, sizeof(std), 1, temp);
            else if (std.id == idn)
            {
                gotoxy(52, 6);
                printf("STUDENT FOUND!");
                gotoxy(24, 8);
                printf("\t\t\tSTUDENT INFORMATION");
                gotoxy(36, 10);
                printf("[1] . Enter Student's Name           : ");
                scanf(" %[^\n]", std.name);
                gotoxy(36, 11);
                printf("[2] . Enter Student's Gender         : ");
                scanf(" %[^\n]", std.gender);
                gotoxy(36, 12);
                printf("[3] . Enter Student's Date Of Birth  : ");
                scanf(" %[^\n]", std.dob);
                gotoxy(36, 13);
                printf("[4] . Enter Student's Phone Number   : ");
                scanf(" %[^\n]", std.phone);
                gotoxy(36, 14);
                printf("[5] . Enter Student's E-mail         : ");
                scanf(" %[^\n]", std.email);
                gotoxy(36, 15);
                printf("[6] . Enter Student's Address        : ");
                scanf(" %[^\n]", std.address);
                gotoxy(36, 16);
                printf("[7] . Enter Student's Department     : ");
                scanf(" %[^\n]", std.dept);
                gotoxy(36, 17);
                printf("[8] . Modify ID (Only If Needed)     : ");
                scanf(" %lld", &std.id);


                gotoxy(24, 20);
                printf("\t\t\tGUARDIUAN INFORMATION");

                gotoxy(36, 22);
                printf("[1] . Enter Student's Father's Name  : ");
                scanf(" %[^\n]", std.fname);
                gotoxy(36, 23);
                printf("[2] . Enter Father's Phone Number    : ");
                scanf(" %[^\n]", std.fphone);
                gotoxy(36, 24);
                printf("[3] . Enter Student's Mother's Name  : ");
                scanf(" %[^\n]", std.mname);
                gotoxy(36, 25);
                printf("[4] . Enter Mother's Phone Number    : ");
                scanf(" %[^\n]", std.mphone);

                fwrite(&std, sizeof(std), 1, temp);
            }
        }
        fclose(fp);
        fclose(temp);
        gotoxy(45, 27);
        printf("STUDENT RECORD HAS BEEN UPDATED");
    }
    else if (check(idn) == 0)
    {
        system("CLS");
        gotoxy(43, 7);
        printf("NO STUDENT FOUND!!!");
        gotoxy(44, 9);
        printf("[1] . Try Again");
        gotoxy(44, 10);
        printf("[2] . Return To Menu");
        gotoxy(44, 11);
        printf("[3] . Exit\n");
        gotoxy(44, 13);
        printf("Please Enter Your Choice [1-3] : ");
        int key;
        scanf("%d", &key);
        if (key == 1)
        {
            system("CLS");
            std_modify();
        }
        else if (key == 2)
        {
            system("CLS");
            adminMenu();
        }

        else if (key == 3)
        {
            exit(1);
        }
    }
    remove("record.txt");
    rename("temp.txt", "record.txt");

    gotoxy(42, 29);
    printf("Press [ENTER] To Return Home");

    int key = getch();
    if (key == 13)
    {
        adminMenu();
    }
}

void std_delete()
{
    system("CLS");
    FILE *fp, *temp;
    long long idn;

    gotoxy(48, 4);
    printf(" DELETE STUDENT RECORD ");
    gotoxy(41, 9);
    printf("Enter Student ID To Delete : ");
    scanf("%lld", &idn);
    if (check(idn) == 1)
    {
        fp = fopen("record.txt", "rb");
        temp = fopen("temp.txt", "wb");
        while (fread(&std, sizeof(std), 1, fp))
        {
            if (std.id == idn)
            {
                gotoxy(47, 9);
                printf(" STUDENT DETAILS");
                gotoxy(36, 11);
                printf("[1] . Name                   : %s", std.name);
                gotoxy(36, 12);
                printf("[2] . ID                     : %lld", std.id);
                gotoxy(36, 13);
                printf("[3] . Department             : %s", std.dept);
                gotoxy(36, 14);
                printf("[4] . Phone Number           : %s", std.phone);

            }
        }

        gotoxy(34, 16);
        printf("Are You Sure You Want To Delete This Student's Record?");
        gotoxy(38, 18);
        printf("[1] . Yes! Delete");
        gotoxy(38, 19);
        printf("[2] . No! Return To Menu");
        gotoxy(36, 21);
        printf("Please Enter Your Choice [1-2] : ");

        int choice;
        scanf("%d", &choice);
        if(choice==1)
        {
            while (fread(&std, sizeof(std), 1, fp))
            {
                if (std.id != idn)
                    fwrite(&std, sizeof(std), 1, temp);
            }
            fclose(fp);
            fclose(temp);
            fp = fopen("record.txt", "wb");
            temp = fopen("temp.txt", "rb");
            while (fread(&std, sizeof(std), 1, temp))
                fwrite(&std, sizeof(std), 1, fp);
            fclose(fp);
            fclose(temp);
            gotoxy(44, 23);
            printf("STUDENT RECORD HAS BEEN DELETED");
            gotoxy(42, 25);
            printf("Press [ENTER] To Return Home");

            int key = getch();
            if (key == 13)
            {
                adminMenu();
            }
        }
        else if(choice==2)
        {
            system("CLS");
            adminMenu();
        }
    }
    else if (check(idn) == 0)
    {
        system("CLS");
        gotoxy(43, 7);
        printf("NO STUDENT FOUND!!!");
        gotoxy(44, 9);
        printf("[1] . Try Again");
        gotoxy(44, 10);
        printf("[2] . Return To Menu");
        gotoxy(44, 11);
        printf("[3] . Exit\n");
        gotoxy(44, 13);
        printf("Please Enter Your Choice [1-2] : ");
        int key;
        scanf("%d", &key);
        if (key == 1)
        {
            system("CLS");
            std_delete();
        }
        else if (key == 2)
        {
            system("CLS");
            adminMenu;
        }

        else if (key == 3)
        {
            exit(1);
        }
    }
}

void deleteAll()
{
    gotoxy(22, 6);
    printf("Are You Sure You Want To Clear System By Deleting All Student's Record?");
    gotoxy(44, 8);
    printf("[1] . Yes! Clear System");
    gotoxy(44, 9);
    printf("[2] . No! Return To Menu");
    gotoxy(40, 11);
    printf("Please Enter Your Choice [1-2] : ");

    int choice;
    scanf("%d", &choice);
    if(choice==1)
    {
        remove("record.txt");
        gotoxy(38, 14);
        printf("SYSTEM HAS BEEN CLEARED SUCCESSFULLY");
        gotoxy(40, 16);
        printf("Press [ENTER] To Return Home");

        int key = getch();
        if (key == 13)
        {
            adminMenu();
        }
    }
    else if(choice==2)
    {
        adminMenu();
    }
}

void std_list()
{
    FILE *fp;
    fp = fopen("record.txt", "rb");
    gotoxy(52, 2);
    printf("STUDENTS LIST");

    gotoxy(2, 4);
    printf("|==================|==============================|==========================|=======================|============|\n");
    gotoxy(2, 5);
    printf("|       ID         |              Name            |           Phone          |       Department      |    CGPA    |\n");
    gotoxy(2, 6);
    printf("|==================|==============================|==========================|=======================|============|\n");
    int y = 7;
    while (fread(&std, sizeof(std), 1, fp))
    {
        gotoxy(2, y);
        printf("|");
        gotoxy(25, y);
        printf("|");
        gotoxy(53, y);
        printf("|");
        gotoxy(80, y);
        printf("|");
        gotoxy(104, y);
        printf("|");
        gotoxy(117, y);
        printf("|");

        gotoxy(9, y);
        printf("%lld", std.id);
        gotoxy(28, y);
        printf("%s", std.name);
        gotoxy(55, y);
        printf("%s", std.phone);
        gotoxy(85, y);
        printf("%s", std.dept);
        gotoxy(107, y);
        printf("%.2lf Tk", std.cgpa);
        gotoxy(2, y+1);
        printf("|----------------------|---------------------------|--------------------------|-----------------------|------------|\n");
        y+=2;
    }
    fclose(fp);

    gotoxy(40, y + 6);
    printf("Press [Enter] To Return Home. ");
    int key = getch();
    if (key == 13)
    {
        adminMenu();
    }
    else
        std_list();
}

void talk_parents()
{
    FILE *fp;
    long long idn;
    gotoxy(50, 2);
    printf(" SEARCH STUDENT ");
    gotoxy(41, 4);
    printf("Enter Student's ID To Search : ");
    scanf("%lld", &idn);
    if (check(idn) == 1)
    {

        while (fread(&std, sizeof(std), 1, fp))
        {
            if (std.id == idn)
            {
                gotoxy(47, 7);
                printf(" STUDENT FOUND ");
                gotoxy(45, 9);
                printf(" STUDENT INFORMATION");
                gotoxy(36, 11);
                printf("[1] . Name                   : %s", std.name);
                gotoxy(36, 12);
                printf("[2] . ID                     : %lld", std.id);
                gotoxy(36, 13);
                printf("[3] . Department             : %s", std.dept);
                gotoxy(36, 14);
                printf("[4] . Phone Number           : %s", std.phone);
                gotoxy(49, 20);
                printf(" PARENTS INFORMATION");
                gotoxy(36, 22);
                printf("[1] . Father's Name          : %s", std.fname);
                gotoxy(36, 23);
                printf("[2] . Mother's Name          : %s", std.mname);
                gotoxy(36, 24);
                printf("[3] . Father's Phone Number  : %s", std.phone);
                gotoxy(36, 25);
                printf("[4] . Mother's Phone Number  : %s", std.phone);
            }
        }
        fclose(fp);
    }
    if (check(idn) == 0)
    {
        system("CLS");
        gotoxy(43, 7);
        printf("NO STUDENT FOUND!!!");
        gotoxy(36, 9);
        printf("[1] . Try Again");
        gotoxy(36, 10);
        printf("[2] . Return To Menu");
        gotoxy(36, 11);
        printf("[3] . Exit\n");
        gotoxy(36, 13);
        printf("Please Enter Your Choice [1-3] : ");
        int key;
        scanf("%d", &key);
        if (key == 1)
        {
            system("CLS");
            talk_parents();
        }
        else if (key == 2)
        {
            system("CLS");
            teacherMenu();
        }

        else if (key == 3)
        {
            exit(1);
        }
    }
    gotoxy(40, 27);
    printf("Press [ENTER] To Return Home");

    int key = getch();
    if (key == 13)
    {
        system("CLS");
        teacherMenu();
    }
    else
    {
        system("CLS");
        talk_parents();
    }
}


int check(long long idn)
{
    FILE *fp;
    fp = fopen("record.txt", "rb");
        if(fp == NULL)
        {
            gotoxy(50,6);
            printf("!!! SYSTEM ERROR !!!");
            gotoxy(45,15);
            exit(1);
        }

    while (!feof(fp))
    {
        fread(&std, sizeof(std), 1, fp);

        if (idn == std.id)
        {
            fclose(fp);
            return 1;
        }
    }
    fclose(fp);
    return 0;
}
