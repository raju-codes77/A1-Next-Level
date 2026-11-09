Title:Generics In Typescript

Introduction:
Generics in Typescript allow us to write reusable code that also support different data types.Instead of writing same function for different type we can use generics.WE use <T> to represent a type that help will be decided later based on the user input or provided data.

Example:
function getResult<T>(value:T):T{
       return value;
}

getResult<string>("abcd")
getResult<number>(10)

Here the same function will work  with strings,numbers or booleans ,we don't need to create two different functions for that.

We can also use Generics with arrays.

       function getResult<T>(value:T[]):T[]{
       return value;
}

getResult<string>(["A","B"]);
getResult<number>([1,2,3]);

The function will work for both data types beacause of generics.

Conclusion:
Generics are an important feature of Typescript.They help us to write flexible and reuseable code while keeping type safety.we can use generics in functions,arrays,objects and classes.It will be useful on large projects or working with apis