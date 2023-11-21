# Intro-To-Java

# Day !
# Day 2
# Day 3
# Day 4
# Day 5 JAva Modifiers

Java provides a number of access modifiers to set access levels for classes, variables, methods, and constructors. 
## The four access levels are:
Visible to the package, the default. No modifiers are needed.
Visible to the class only (private).
Visible to the world (public).
Visible to the package and all subclasses (protected).

## Default Access Modifier - No Keyword
Default access modifier means we do not explicitly declare an access modifier for a class, field, method, etc.
A variable or method declared without any access control modifier is available to any other class in the same package. The fields in an interface are implicitly public static final and the methods in an interface are by default public.
### Example
Variables and methods can be declared without any modifiers, as in the following an example:

String version = "1.5.1";
boolean processOrder() {
   return true;
}

## Private Access Modifier - Private
Methods, variables, and constructors that are declared private can only be accessed within the declared class itself.Private access modifier is the most restrictive access level. Class and interfaces cannot be private.
Variables that are declared private can be accessed outside the class, if public getter methods are present in the class. Using the private modifier is the main way that an object encapsulates itself and hides data from the outside world.

### Example
The following class uses private access control

public class Logger {
   private String format;

   public String getFormat() {
      return this.format;
   }

   public void setFormat(String format) {
      this.format = format;
   }
}
The format variable of the Logger class is private, so there's no way for other classes to retrieve or set its value directly. So, to make this variable available to the outside world, we defined two public methods: getFormat(), which returns the value of format, and setFormat(String), which sets its value.

## Public Access Modifier - Public
A class, method, constructor, interface, etc. declared public can be accessed from any other class. Therefore, fields, methods, blocks declared inside a public class can be accessed from any class belonging to the Java Universe.

However, if the public class we are trying to access is in a different package, then the public class still needs to be imported. Because of class inheritance, all public methods and variables of a class are inherited by its subclasses.

### Example
The following function uses public access control:

Public static void main(String[] arguments) {
}
The main() method of an application has to be public. Otherwise, it could not be called by a Java interpreter (such as java) to run the class.

## Protected Access Modifier - Protected
Variables, methods, and constructors, which are declared protected in a superclass can be accessed only by the subclasses in other package or any class within the package of the protected members' class. The protected access modifier cannot be applied to class and interfaces. Methods, fields can be declared protected, however methods and fields in a interface cannot be declared protected. Protected access gives the subclass a chance to use the helper method or variable, while preventing a nonrelated class from trying to use it.

### Example
The following parent class uses protected access control, to allow its child class override openSpeaker() method:
class AudioPlayer {
   protected boolean openSpeaker(Speaker sp) {
      // implementation details
   }
}

class StreamingAudioPlayer extends AudioPlayer {
   boolean openSpeaker(Speaker sp) {
      // implementation details
   }
}
If we define openSpeaker() method as private, then it would not be accessible from any other class other than AudioPlayer. If we define it as public, then it would become accessible to all the outside world. But our intention is to expose this method to its subclass only, that's why we have used protected modifier.

## Access Control and Inheritance
The following rules for inherited methods are enforced:
1. Methods declared public in a superclass also must be public in all subclasses.
2. Methods declared protected in a superclass must either be protected or public in subclasses; they cannot be private.
3. Methods declared private are not inherited at all, so there is no rule for them.

Example
In this example, we've created a class with a private variable age and a variable with default scope as name. Using setter/getter method, we're updating age and getting value and name is updated directly.

public class Puppy {
   private int age;
   String name;

   public Puppy() {      
   }

   public void setAge( int age ) {
      this.age = age;
   }

   public int getAge( ) {
      return age;
   }

   public static void main(String []args) {
      Puppy myPuppy = new Puppy();

      // update age variable using method call
      myPuppy.setAge( 2 );

      // update name directly
      myPuppy.name = "Tommy";
      System.out.println("Age: " + myPuppy.getAge() +", name: " + myPuppy.name );
   }
}
Output

Age: 2, name: Tommy
# =====================================================================================================================================week 2====================================================================================================================================================================

# Day 1
# Day2
Git is a distributed revision control and source code management system with an emphasis on speed. Git was initially designed and developed by Linus Torvalds for Linux kernel development. Git is a free software distributed under the terms of the GNU General Public License version 2. This tutorial explains how to use Git for project version control in a distributed environment while working on web-based and non web-based applications development. We can  use Git to handle all levels of Java and Non-Java projects. So an exposure to software development life cycle and working knowledge of developing web-based and non web-based applications is a good start to work with GIt tools.Git comes with some tools like Git Bash, Git GUI to provide the interface between machine and user. It supports inbuilt as well as third-party tools.Git comes with built-in GUI tools like git bash, git-gui, and gitk for committing and browsing. It also supports several third-party tools for users looking for platform-specific experience.
Git Package Tools
Git provides powerful functionality tools such as commands, command line, Git GUI. Let's have a glimpse of some essential package tools.
GitBash
Git Bash is an application for the Windows environment. It is used as Git command line for windows. Git Bash provides an emulation layer for a Git command-line experience. Bash is an abbreviation of Bourne Again Shell. Git package installer contains Bash, bash utilities, and Git on a Windows operating system.
Git Bash Commands
Git Bash comes with some additional commands that are stored in the /usr/bin directory of the Git Bash emulation. Git Bash can provide a robust shell experience on Windows. Git Bash comes with some essential shell commands like Ssh, scp, cat, find.

Git Bash also includes the full set of Git core commands like git clone, git commit, git checkout, git push, and more.

Git GUI
Git GUI is a powerful alternative to Git BASH. It offers a graphical version of the Git command line function, as well as comprehensive visual diff tools. We can access it by simply right click on a folder or location in windows explorer. Also, we can access it through the command line by typing below command.
