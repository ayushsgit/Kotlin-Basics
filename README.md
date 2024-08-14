# Kotlin-Basics
Fundamentals of Kotlin programming Language

import java.util.*

fun main(){
    println("hello World!!!") // prints hello World!!!

    //Variables
    val firstName = "Ayush"   //val = read only variable
    var weight = 154          //var = read and write variable
    val myVariable : Double = 22.3
    val myVari : Boolean = true

    //Operators
    val s1 = "Call me"
    val s2 = " maybe"
    val combined = s1 + s2 // concatenation
    println(s1 + s2)

    val n1 = 5
    val n2 = 8
    val result = n1 - n2
    println(result)

    //STRINGS
    val myString = "KOTLIN"
    println(myString[0])
    println(myString[1])
    println(myString.isEmpty())
    println(myString.length)
    println(myString.substring(2, 4))
    println("The string is $myString")

    //Conditionals
    val examScore = 96
    if(examScore > 70){
        println("You Passed!!")
    } else{
        println("You Failed")
    }

    //Collections
//    val name1 = "May"
//    val name2 = "June"
//    val name3 = "July"
    val names = listOf("May", "June", "July")
    println(names[2]) //kotlin is zero indexed

    val NAMES = mutableListOf("May", "June", "July")
    NAMES.add("August")
//    NAMES.add(50) only same data type can be added
    println(NAMES)

    //for loops
    for(name in NAMES){
        println(NAMES)
    }

    for(i in 1..5){ //to include the last number i.e. 55
        println(i)
    }

    for(i in 1 until 5){ //not include the last number i.e. 5
        println(i)
    }

    // nullability : no value
    val Instagram : String? = null //nullable string
    if(Instagram != null){
        println(Instagram.uppercase()) //No Output will be printed
    }
    val InstagramBio : String? = "grow" //nullable string
    if(InstagramBio != null){
        println(InstagramBio.uppercase()) //Output will be printed
    }

    println(InstagramBio?.uppercase()) // checks if variable value is not null then proceeds
    //method i.e. uppercase() is only called when this variable/object i.e. InstagramBio is not null

    myFunction("Luffy")
}

//Functions
fun myFunction(name : String){
    println("Hello this is my Function and my name is $name")
}

//Private Functions : Cannot be accessed from other classes or files
private fun myFun(name : String){
    println("Hello this is my Function and my name is $name")
}

%% /home/luffy/.jdks/openjdk-20.0.2/bin/java -javaagent:/home/luffy/idea-IC-232.9921.47/lib/idea_rt.jar=45385:/home/luffy/idea-IC-232.9921.47/bin -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath /home/luffy/IdeaProjects/AppKotlin/out/production/AppKotlin:/home/luffy/.m2/repository/org/jetbrains/kotlin/kotlin-stdlib-jdk8/1.9.0/kotlin-stdlib-jdk8-1.9.0.jar:/home/luffy/.m2/repository/org/jetbrains/kotlin/kotlin-stdlib/1.9.0/kotlin-stdlib-1.9.0.jar:/home/luffy/.m2/repository/org/jetbrains/kotlin/kotlin-stdlib-common/1.9.0/kotlin-stdlib-common-1.9.0.jar:/home/luffy/.m2/repository/org/jetbrains/annotations/13.0/annotations-13.0.jar:/home/luffy/.m2/repository/org/jetbrains/kotlin/kotlin-stdlib-jdk7/1.9.0/kotlin-stdlib-jdk7-1.9.0.jar MainKt
hello World!!!
Call me maybe
-3
K
O
false
6
TL
The string is KOTLIN
You Passed!!
July
[May, June, July, August]
[May, June, July, August]
[May, June, July, August]
[May, June, July, August]
[May, June, July, August]
1
2
3
4
5
1
2
3
4
GROW
GROW
Hello this is my Function and my name is Luffy

Process finished with exit code 0
%%
