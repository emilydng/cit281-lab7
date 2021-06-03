## Lab 7

``` markdown
Goals and Outcomes

  -  Install and setup your personal computer with the software tools required for this course
  -  Practice using software tools
  -  Practice terminal or shell commands
  -  Practice keyboard shortcuts
  -  Create your first Node.js server-side JavaScript file

```

Lab-07.js

```rouge
   /*
    CIT 281 Lab 07
    Emily Deng
  */

  class CustomError extends Error {
      constructor(args) {
          super(args);
          this.name = "CustomError";
      }
  };

  function throwGenericError() {
      throw new Error("Generic error");
  }

  function throwCustomError() {
      throw new CustomError("Custom error");
  }

  console.log("Force generic error");
  try {
      console.log("Generic error try block");
      throwGenericError();
  } catch (error) {
      console.log("Generic error catch block");
      console.log(`${error.name}: ${error.message}`);
  } finally {
      console.log("Generic error finally block");
  }

  console.log("Force custom error");
  try {
      console.log("Custom error try block");
      throwCustomError();
  } catch (error) {
      console.log("Custom error catch block");
      console.log(`${error.name}: ${error.message}`);
  } finally {
      console.log("Custom error finally block");
  }

 ```
 
 *Screencapture of GitHub repo page*

<img width="718" alt="lab-07" src="https://user-images.githubusercontent.com/84113983/120716184-86b51280-c47a-11eb-9c9e-1a9f9dc36465.png">


