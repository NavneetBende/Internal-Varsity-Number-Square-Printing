PRINTING PATTERN:
333

313

323

333

PREREQUISITE:
Basic knowledge of C language and loops.

ALGORITHM:
Take number of rows as input from the user and save it in any variable (‘r’in this case).
Run a loop ‘r’ number of times to iterate through the rows. From i=0 to i<r.  The loop should be structured as for( i=0 ; i<r ; i++).
Inside this if condition use an id condition to print the top and bottom rows. if(i==0 || i==r-1).
Inside this run a nested loop to iterate through the columns. From  j=0 to j<3. The loop should be structured as for(j=0 ; j<3 ; j++).
Print “3” in this loop.
Write an else condition. Inside it a run a similar loop . From  j=0 to j<3. The loop should be structured as for(j=0 ; j<3 ; j++).
Use an if condition. if(j==0 || j==2). And  print “3”.
Else print the iterating variable for rows.
Inside the main loop print a newline
CODE IN C:
#include<stdio.h>
int main()
{
int i,j,r;                                          //declaring integer variables i,j for loops , r for number of rows
printf("Enter the number of rows :\n");             //asking user for input
scanf("%d",&r);                                     //saving number of rows in variable r
for(i=0;i<r;i++)                                    //loop for number of rows
   {
      if(i==0 || i==r-1)                            //if condition to print first and last row
         {
            for(j=0;j<3;j++)                        //loop to print first and last row
               {
                  printf("3");                      //printing 3
               }
         }
      else                                          //else to print rest of the square
         {
            for(j=0;j<3;j++)                        //loop to print the rest of the square
              {
                  if(j==0 || j==2)                  //if condition to print the outer values
                     {
                        printf("3");                //printing 3
                     }
                  else//else condition to
                     {
                        printf("%d",i);              //Printing the middle column
                     }
              }
         }
      printf("\n");                                  //printing newline
   }
}
TAKING INPUT:
DISPLAYING OUTPUT:
