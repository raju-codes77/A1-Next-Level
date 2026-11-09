Title:Type Vs Interface
Introduction:
Typescript provides two ways to describe the structure of data.They tell us what kind of data we can use and what properties an object should.They both work almost the same way but they have some differences.

Detailed Body:
An interface is mainly used to describe the structure of an object.
Example:
       interface User{
              name:string;
              age:number;
       }
       Here every user must have a name and an age otherwise it will throw an error.

       Type also describe an object

       type user={
              name:string;
              age:number;
       }
       Here we can see a visual differences that we need to use = sign for written the type alias .

       Both example do the same thing.

       Main Differences:
       extending, For that interface uses extends,while type uses & to combine two structures;
       Example:
              interface Admin Extends user{
                     role:string;
              }

              type Admin=user &{
                     role:string;
              }

              Union Type:
              Type support union types but interface can not directly do this.

Conclusion:
Both Type and Interface are useful in typescript.There is no strict rule about which one to use.We can choose them based on our project needs that would be useful and flexible for the project.