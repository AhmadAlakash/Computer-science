 #include <stdio.h>
#include <cs50.h>
int main(void){
   // string answer = get_string("What's your name");
   // printf("Hallo,%s \n",answer);
   // bool answer2 = get_bool()
    int num1 = 10 ;
    int num2 = 20 ;
   // printf("%i\n%i\n", num1,num2); // to print our values
   // printf("%i\n", num1+num2); // to count our values
   // printf("%i\n", num2-num1); // to count our values
   // printf("%i\n", num2/num1); // to count our values
   // printf("%i\n", num1*num2); // to count our values
  //  printf("%i\n", num2%num1); // to count our values
    printf("%i\n",1+num1); //to add 1 of values
    printf("%i\n",++num1); //to add 1 of values
    printf("%i\n",--num1); //to add 1 of values



}
-------------------------------------------------------------------------


Command line functions :

code mario.c to create file

rm mario.c to delete file

ls to know how much files we have

mkdir to ؤreate folder

rmdir to delete folder

mv x newx to rename file

../../newx  to play  file from our place


----------------------------------------------------------------------

function take two numbers and calc and give the result

// not bad but not the best
  //  int num1 = get_int("Enter your number to calc : ");
  //  int num2 = get_int("Enter your number to calc : ");
//    int result = num1 +num2 ;
 //   printf("%i\n",num1 + num2);
    // when i have grate value most  long use

  btter than the first :
    int num1 = get_int("num1 : ");
    int num2 = get_int("num2 : ");
    printf("%i\n",num1+num2);



}

------------------------------------------------------------------

comparison :


  int x = get_int("x : ");
   int y = get_int("y : ");

   if (x<y)
   {
    printf("x is less than y ");
   }
   else if(x>y)
   {
    printf("x is grater than y ");
   }
   else{
    printf("x is equal y ");
   }

}

--------------------------------------------------------------------
app show if the num even or odd

  int n = get_int("n : ") ;

  if (n % 2 == 0)
  {
    printf("even\n");
  }
  else{
    printf("odd\n");
  }
}
--------------------------------------------------------------------

Agree موافق على

app ask the user if he agree or not :

or in c is ||


 char c = get_char("Do you agree y/n : ") ;

 if (c == 'y'|| c ==  'Y')
    {
      printf("agree");

    }
 else if (c == 'n' || c == 'N')
    {
      printf("not agree");

      }
}

-------------------------------------------------
Loops :

wihle :

int i = 0 ;    start
 while (i <= 3)  condition
 {
  printf("Hadil\n")
  i += 1
  i = i+1
  i++        steps
 }

int i = 0 ;
 while (i <= 3)
 {
  printf("%i\n",i)
 }

------------------

 for :


 for (start ;  condition  ; steps  )
      {
        prinf() ;
      }



App write from 0 to 10  just even num  with for and with while :

printf("--------------FOR----------------\n");

for(int i = 0 ; i<11;i+=2)
  {printf("%i\n",i);
  }

printf("---------------WHILE---------------\n");
  int i = 0 ;
  while (i<11)
    {
      printf("%i\n",i);
      i+=2;
    }

------------------------------------------------------------------------------

Functions :

using :


big problem  and just in the int main (void){         is to difficult but but when we use the functions and
the bi problem to small problem + smal problem + smal problem >>>>is easy as what we had

}


ex : company has so much people for work not just one


we write the another functions above the int main function

--------------------
#include <stdio.h>
#include <cs50.h>



void hello (void){                             !!!! void mean than this empty !!!!!

     printf("ALSALAM Alekum");
}




int main (void){

    hello()

}
--------------------------


#include <stdio.h>
#include <cs50.h>



void hello (int n){

     printf("ALSALAM Alekum");
}




int main (void){

    hello()

}

 when will write one or more functions down from the main we need to main tell this and that is by the write above the main  identification





#include <stdio.h>
#include <cs50.h>



void hello (void){

     printf("ALSALAM Alekum\n");
}


void meow(int n){
  for(int i = 0 ; i<n;i++)

      printf("meow\n");
}

void sum(int n1 , int n2){
    int result=n1+n2;
    printf("%i\n",result);
}




int main (void){

    hello();
    meow(6);
    sum(500,1000);
    sum(500,4566);
}
 --------------------------------------------
EX :    project

- simple project
- create dicount function
- super function
- percent

write programm get number from user for price  and make discount of this price 15 %



#include <stdio.h>
#include <cs50.h>


 /*
  shape 1 :
  int main (void){

  float regular = get_float("Enter Your Price : ");
  float sale = regular*.85;
  printf(" your new price with discount : %.2f\n",sale);


}
*/

/*
Shape 2:



      float regular = get_float("Enter your regular Price to make discount : ");
      float sale = discount(regular);
      printf("New Price with discount : %.2f\n",sale);

}

float discount(float price ){

     float sale = price * .85;
     return sale ;
we can with just one line this :


float discount(float price ){
  retur price*.85;




*/

/*
shape 3 here i will from user the price and the percent :



    float regular = get_float("Enter your price : ");
    float percent = get_float("Enter your percent : ");
    float sale = discount(regular,percent);
    printf("New price : %.2f\n",sale);







}
float discount(float price,float percent){
  return price*(100-percent)/100;   >>>>>this opertion for give the .85!!!!!!!

}
*/

---------------------------------------------------------------------------------------------------------

code write "?" as in the Mario




int main (void){

// code write for you (?) as you will

int count = get_int("Enter your number : ");
for  (int i = 0 ;i<count; i++)
    printf("?");

printf("\n");


int sum = get_int("Enter number please : ") ;
int i = 0;

while ( i < sum ){
    printf("#");
    i++;
}
printf("\n");
}

-------------------------------------------------------------------------


int main (void){

// code write for you (?) as you will

int count = 0;

while (count <1 ){


    count = get_int("Enter your number : ");
}
for  (int i = 0 ;i<count; i++)
    printf("?");

printf("\n");



}
-----------------------------------------------------------------------------------

int main (void){

// code write for you (?) as you will

int count;
do {

    count = get_int("Enter your number : ");

}while (count < 1);


for  (int i = 0 ;i<count; i++)
    printf("?");

printf("\n");



}
----------------------------------------------------------------------------------------------------------

#include <stdio.h>
#include <cs50.h>


int main (void){

// code write for you (?) as you will
int count;       // definition varibles
do {              // do it for once
    count = get_int("Enter number : ");

}while(count<1);   // condition



}



for (int i = 0;i<count;i++){
    for (int j = 0 ;j<count;j++){
            printf("#");

    }
    printf("\n");

}

-----------------------------------------------------------------------------------


#include <stdio.h>
#include <cs50.h>


int main (void){

    /*
    قسمة الاعداد الصحيحة والتحويل من قيمة الى قيمة
    */

   int x = get_int("x : ");
   int y = get_int("y : ");

   printf("%f \n", (double)x/(double)y);






}


------------------------------------------------------------------------------


#include <stdio.h>
#include <cs50.h>


int main (void){

    // لتثبيت قيمة متغير ومنع تغييره const 
    
    const int i = 50;
    i = 30;
    printf("%i",i);


/* سيظهر خطا بسبب محاولة تغيير متغير قيمته ثابتة */

}


-----------------------------------------------------------------------------------