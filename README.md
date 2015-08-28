# Inner-class

Advantage of Inner class:

      1.Better encapsulation. Innver class can only be accessed by its outer class. The other classes in the package cannot           access this inner class.

      2.Inner class can be accessed to the field in outer class, even the private filed.

      3.sometimes more convenient.

        Note: outter class cannot access inner class derectly. We can create a new object of inner class and then access its          method.

types of Inner class:

    Member Inner Class/成员内部类:

      1、 Inner 类可以使用任意访问控制符，如 public 、 protected 、 private 等

      2、 method in Inner class can access the field in Outter class even if it's private.

      3、 create a innner class object: InnerClass ic = new OutterClass.InnerClass();

      4、 After compiling, we have two files: Outer$Inner.class , Outter.class


   Static Nested Classes:

      1. static nested class cannot access the non-static field directly, but can use: new Outer().field.

      2. If name of static field of outer class is same as the field of inner class, in the method of inner class, we can           use:outer.staticfield; If not same, we can access the field directly.

      3. Create the inner class object, just use constructor directly without outer class: Inner obj = new Inner();

   Method-Local Inner Classes
      1. it can be only used in the method


   Anonymous Classes
      1. Anonymous classes enable you to make your code more concise. 

      HelloWorld frenchGreeting = new HelloWorld() {
            String name = "tout le monde";
            public void greet() {
                greetSomeone("tout le monde");
            }
