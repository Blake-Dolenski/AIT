# AIT
Swift

--Instances--
Instances of a structure are independent of each other.
When creating an instance of a data structure, the datatype of that structure is the name after the struct.
EX:
struct MyStructure() {
var msg = "hi"
  func myFunction(){
    print(msg)
  }
}

--Property--
A property is another name for a variable inside a structure.
You can access properties and methods of a structure by using the dot-notation on an instance of a structure

--Modifier--
A modifier changes the look and behavior of a view element

--Function--
A function is a block of code with a name (function declaration) that can be executed when called by name (function call)
A method is what a function is called when it is in a structure
self refers to a current instance in the body of one of its methods
EX:
func myFunc( _ a: Int, _ b: Int=0) -> Int {
return a+b
}
myFunc(1,2)
OUTPUT: 3

func myFunc(a:Int, b:Int)->Int{
        return a+b
        print("thanks")
}
print("the sum is ", myFunc(a:3, b:5))
OUTPUT: the sum is 8

--Structure--
A structure is a way to organize your code to model or represent something (a view, a role, a component) in your app
Structures can be used to represent a View (e.g., screen).
In Swift, structs are value types whereas classes are reference types. When you copy a struct, you end up with two unique copies of the data. When you copy a class, you end up with two references to one instance of the data. It's a crucial difference, and it affects your choice between classes or structs.
The datatype of a structure is the name of the structure itself


--Variables--
Variables declared inside a function won't exist outside a function. This is called variable scope.
When you don't specify a data type for your variable the variable will infer the data type from the first piece of data you assign to it.

--Images--
When specifying the image to display for an image element, add the image to the asset library and specify the asset name in between the parentheses of your image element
The App icon should be a 1024 x 1024 png image

--enum--
an enum (short for "enumeration") is a data type that allows you to define a group of related values. Enums are commonly used to represent a fixed set of values or options that a variable or function parameter can take.

--@State--
When we put @State before a property, we effectively move its storage out from our struct and into shared storage managed by SwiftUI.
SwiftUI uses the @State property wrapper to allow us to modify values inside a struct, which would normally not be allowed because structs are value types.

--@Published--
@Published is one of the property wrappers in SwiftUI that allows us to trigger a view redraw whenever changes occur. You can use the wrapper combined with the ObservableObject protocol, but you can also use it within regular classes.

--Tools--
Inspector Panel: For looking at details or customizing the attributes of what you select in the Editor area
HStack: Container that holds items in a horizontal line
VStack: Container that holds items in a vertical line
ZStack: Container that holds items in a 3-D view (Overlays views on top of each other)
All containers are limited to 10 children
Lazy ZStack: A conatiner just like a ZStack but it only shows what the user wants to see and doesn't rendor anymore

