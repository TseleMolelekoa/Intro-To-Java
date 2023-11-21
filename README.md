# Intro-To-Java
# WEEK 1 
# Day 1


What is java? 

Java is a general-purpose programming language that is class-based, object-oriented, and designed to have as few implementation dependencies as possible. It is intended to let application developers write once, run anywhere (WORA), meaning that compiled Java code can run on all platforms that support Java without the need for recompilation. JAVA was developed by Sun Microsystems Inc and first released in 1991, later acquired by Oracle Corporation. 

 

 

Java Components 

Java Virtual Machine (JVM) 

Generally referred as JVM, it’s the primary function is to execute the bytecode produced by compiler. 

Java Development Kit (JDK) 

This is a complete java development kit that includes JRE (Java Runtime Environment), compilers and various tools like JavaDoc, Java debugger etc. 

Java Runtime Environment (JRE) 

JRE allows you to run java programs, it includes JVM, browser plugins and applets support. When you only need to run a java program on your computer, you would only need JRE. 

 

Main Java features 

Platform Independence: 

Java is designed to be platform-independent, meaning that Java programs can run on any device with a compatible Java Virtual Machine (JVM). 

Object-Oriented Programming (OOP): 

Java is a fully object-oriented programming language, emphasizing concepts such as encapsulation, inheritance, and polymorphism. 

Simple and Easy to Learn: 

Java was designed to be straightforward and easy to learn for programmers. It eliminates complex features such as pointers, operator overloading, and multiple inheritance, making it more accessible for developers. 

Robust and Secure: 

Java incorporates features like strong memory management, exception handling, and a comprehensive set of APIs, which contribute to the robustness and reliability of Java applications. 

Multithreading: 

Java supports multithreading, allowing concurrent execution of multiple threads within a program. 

 

Install Java Development Kit (JDK): 

Visit the Oracle JDK download page or OpenJDK to download and install the latest version of the Java Development Kit (JDK). Follow the installation instructions for your operating system. 

 

Set the JAVA_HOME environment variable: 

On Windows: Right-click on "This PC" or "Computer," select "Properties," click on "Advanced system settings," go to the "Advanced" tab, and click "Environment Variables." Add a new system variable with the name JAVA_HOME and the path to your JDK installation (e.g., C:\Program Files\Java\jdk1.8.0_291). 

Typical Structure of a Java program 

A typical structure of a Java program contains the following elements: 

Package declaration 

Import statements 

Comments 

Class definition 

Attributes 

Methods/Behaviours 

 



# Day 2

DAY 2 

 

What is a variable? 

A variable is a name given to a memory location. It is the basic unit of storage in a program. 

The value stored in a variable can be changed during program execution. 

A variable is only a name given to a memory location; all the operations done on the variable effects that memory location. 

In Java, all the variables must be declared before use. 

How to declare variables? 

type: Type of data that can be stored in this variable. 

name: Name given to the variable. 

It can be assigned values in two ways: 

Variable Initialization 

Assigning value by taking input. 

 

Declaring and initialize variables: 

datatype: Type of data that can be stored in this variable. 

variable_name: Name given to the variable. 

value: It is the initial value stored in the variable. 

Declaring variables examples 

float simpleInterest; - Declaring float variable 

int myAge = 19; - Declaring and Initializing integer variable 

char firstLetter = 'h'; - Declaring and Initializing character variable 

 

 

There are three types of variables in Java: 

 

Local Variables: A variable defined within a block or method or constructor is called local variable. 

Instance Variables: Instance variables are non-static variables and are declared in a class outside any method, constructor or block. 

Static Variables: Static variables are also known as Class variables. 

## Data types in Java: 

1) Primitive data types - A primitive data type specifies the size and type of variable values, and it has no additional methods. 

2)  Non-primitive data types – Arrays and Strings are non-primitive data types, these are the datatypes which have instances like objects. Hence, they are called reference variables. They are primarily classes, arrays, strings or interfaces. 



There are eight primitive data types in Java: 

Byte 

Short 

Int 

Long 

Float 

Double 

Boolean 
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
Git facilitates with some built-in GUI tools for committing (git-gui) and browsing (gitk), but there are many third-party tools for users looking for platform-specific experience.

Gitk
gitk is a graphical history viewer tool. It's a robust GUI shell over git log and git grep. This tool is used to find something that happened in the past or visualize your project's history.

Gitk can invoke from the command-line. Just change directory into a Git repository, and type:

$ gitk [git log options]
# According to Tutorialspoint : 
# Version Control System
Version Control System (VCS) is a software that helps software developers to work together and maintain a complete history of their work.
Listed below are the functions of a VCS : 
1. Allows developers to work simultaneously.
2. Does not allow overwriting each other’s changes.
3. Maintains a history of every version.

Following are the types of VCS :
1. Centralized version control system (CVCS).
2. Distributed/Decentralized version control system (DVCS).

# Distributed Version Control System
Centralized version control system (CVCS) uses a central server to store all files and enables team collaboration. But the major drawback of CVCS is its single point of failure, i.e., failure of the central server. Unfortunately, if the central server goes down for an hour, then during that hour, no one can collaborate at all. And even in a worst case, if the disk of the central server gets corrupted and proper backup has not been taken, then you will lose the entire history of the project. Here, distributed version control system (DVCS) comes into picture.

DVCS clients not only check out the latest snapshot of the directory but they also fully mirror the repository. If the server goes down, then the repository from any client can be copied back to the server to restore it. Every checkout is a full backup of the repository. Git does not rely on the central server and that is why you can perform many operations when you are offline. You can commit changes, create branches, view logs, and perform other operations when you are offline. You require network connection only to publish your changes and take the latest changes.

DVCS Terminologies
Local Repository
Every VCS tool provides a private workplace as a working copy. Developers make changes in their private workplace and after commit, these changes become a part of the repository. Git takes it one step further by providing them a private copy of the whole repository. Users can perform many operations with this repository such as add file, remove file, rename file, move file, commit changes, and many more.

Working Directory and Staging Area or Index
The working directory is the place where files are checked out. In other CVCS, developers generally make modifications and commit their changes directly to the repository. But Git uses a different strategy. Git doesn’t track each and every modified file. Whenever you do commit an operation, Git looks for the files present in the staging area. Only those files present in the staging area are considered for commit and not all the modified files.

Let us see the basic workflow of Git.

Step 1 − You modify a file from the working directory.

Step 2 − You add these files to the staging area.

Step 3 − You perform commit operation that moves the files from the staging area. After push operation, it stores the changes permanently to the Git repository.

### Git Tutorial
Suppose you modified two files, namely “sort.c” and “search.c” and you want two different commits for each operation. You can add one file in the staging area and do commit. After the first commit, repeat the same procedure for another file.

# First commit
[bash]$ git add sort.c

# adds file to the staging area
[bash]$ git commit –m “Added sort operation”

# Second commit
[bash]$ git add search.c

# adds file to the staging area
[bash]$ git commit –m “Added search operation”

## Blobs
Blob stands for Binary Large Object. Each version of a file is represented by blob. A blob holds the file data but doesn’t contain any metadata about the file. It is a binary file, and in Git database, it is named as SHA1 hash of that file. In Git, files are not addressed by names. Everything is content-addressed.

## Trees
Tree is an object, which represents a directory. It holds blobs as well as other sub-directories. A tree is a binary file that stores references to blobs and trees which are also named as SHA1 hash of the tree object.

## Commits
Commit holds the current state of the repository. A commit is also named by SHA1 hash. You can consider a commit object as a node of the linked list. Every commit object has a pointer to the parent commit object. From a given commit, you can traverse back by looking at the parent pointer to view the history of the commit. If a commit has multiple parent commits, then that particular commit has been created by merging two branches.

## Branches
Branches are used to create another line of development. By default, Git has a master branch, which is same as trunk in Subversion. Usually, a branch is created to work on a new feature. Once the feature is completed, it is merged back with the master branch and we delete the branch. Every branch is referenced by HEAD, which points to the latest commit in the branch. Whenever you make a commit, HEAD is updated with the latest commit.

## Tags
Tag assigns a meaningful name with a specific version in the repository. Tags are very similar to branches, but the difference is that tags are immutable. It means, tag is a branch, which nobody intends to modify. Once a tag is created for a particular commit, even if you create a new commit, it will not be updated. Usually, developers create tags for product releases.

## Clone
Clone operation creates the instance of the repository. Clone operation not only checks out the working copy, but it also mirrors the complete repository. Users can perform many operations with this local repository. The only time networking gets involved is when the repository instances are being synchronized.

## Pull
Pull operation copies the changes from a remote repository instance to a local one. The pull operation is used for synchronization between two repository instances. This is same as the update operation in Subversion.

## Push
Push operation copies changes from a local repository instance to a remote one. This is used to store the changes permanently into the Git repository. This is same as the commit operation in Subversion.

## HEAD
HEAD is a pointer, which always points to the latest commit in the branch. Whenever you make a commit, HEAD is updated with the latest commit. The heads of the branches are stored in .git/refs/heads/ directory.

[CentOS]$ ls -1 .git/refs/heads/
master

[CentOS]$ cat .git/refs/heads/master
570837e7d58fa4bccd86cb575d884502188b0c49
## Revision
Revision represents the version of the source code. Revisions in Git are represented by commits. These commits are identified by SHA1 secure hashes.

## URL
URL represents the location of the Git repository. Git URL is stored in config file.

[tom@CentOS tom_repo]$ pwd
/home/tom/tom_repo

[tom@CentOS tom_repo]$ cat .git/config
[core]
repositoryformatversion = 0
filemode = true
bare = false
logallrefupdates = true
[remote "origin"]
url = gituser@git.server.com:project.git
fetch = +refs/heads/*:refs/remotes/origin/*

Use git merge when you want to keep a clear record of when and where changes were merged. Merging is a safe option and is appropriate for public branches.

Use git rebase when you want to create a more linear and cleaner commit history. This is beneficial for feature branches, but be cautious when rebasing commits that have been pushed to a shared repository, as it rewrites history.


# Day 3
# Day 4
# Day 5
