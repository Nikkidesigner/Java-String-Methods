Java String Class Methods
The java.lang.String class provides a lot of built-in methods that are used to manipulate string in Java. By the help of these methods, we can perform operations on String objects such as trimming, concatenating, converting, comparing, replacing strings etc.

Java String is a powerful concept because everything is treated as a String if you submit any form in window based, web based or mobile application.
//-----------------------------------------------------------

Java String toUpperCase() and toLowerCase() method
The Java String toUpperCase() method converts this String into uppercase letter and String toLowerCase() method into lowercase letter.

Stringoperation1.java

public class Stringoperation1  
{  
public static void main(String ar[])  
{  
String s="Sachin";    
System.out.println(s.toUpperCase());//SACHIN    
System.out.println(s.toLowerCase());//sachin    
System.out.println(s);//Sachin(no change in original)    
}  
}  
Output:

SACHIN
sachin
Sachin

//------------------------------------------------------------

Java String trim() method
The String class trim() method eliminates white spaces before and after the String.

Stringoperation2.java

public class Stringoperation2  
{  
public static void main(String ar[])  
{  
String s="  Sachin  ";    
System.out.println(s);//  Sachin      
System.out.println(s.trim());//Sachin    
}  
}  
Output:

Sachin  
Sachin

//------------------------------------------------------------

Java String startsWith() and endsWith() method
The method startsWith() checks whether the String starts with the letters passed as arguments and endsWith() method checks whether the String ends with the letters passed as arguments.

Stringoperation3.java

public class Stringoperation3  
{  
public static void main(String ar[])  
{  
String s="Sachin";    
 System.out.println(s.startsWith("Sa"));//true    
 System.out.println(s.endsWith("n"));//true    
}  
}  
Output:

true
true

//------------------------------------------------------------

Java String charAt() Method
The String class charAt() method returns a character at specified index.

Stringoperation4.java

public class Stringoperation4  
{  
public static void main(String ar[])  
{  
String s="Sachin";    
System.out.println(s.charAt(0));//S    
System.out.println(s.charAt(3));//h    
}  
}  
Output:

S
h

//------------------------------------------------------------

Java String length() Method
The String class length() method returns length of the specified String.

Stringoperation5.java

public class Stringoperation5  
{  
public static void main(String ar[])  
{  
String s="Sachin";    
System.out.println(s.length());//6    
}  
}  
Output:

6

//------------------------------------------------------------

Java String replace() Method
The String class replace() method replaces all occurrence of first sequence of character with second sequence of character.

Stringoperation8.java

public class Stringoperation8  
{  
public static void main(String ar[])  
{  
String s1="Java is a programming language. Java is a platform. Java is an Island.";      
String replaceString=s1.replace("Java","Kava");//replaces all occurrences of "Java" to "Kava"      
System.out.println(replaceString);    
}  
}     
Output:

Kava is a programming language. Kava is a platform. Kava is an Island.

//------------------------------------------------------------
following are more methods in string , stringbuffer and string builder :

class  StringMethods
{
	public static void main(String[] args) 
	{
		String name = "           Nikhil Rajesh Pawar     ";
		String emp = "";
		String S1 = "Nikhil";
		String S2 = "Nikhil";
		String S3 = "NIKHIL";
		String S4 = "Pawar";
		String S5 = "PAWAR";
		String S = "This is demo";

		System.out.println(" trim() method to remove empty spaces : "+name.trim());
		
		System.out.println("\n equals method (S1 and S2): "+S1.equals(S2));

		System.out.println("\n equalsIgnoreCase method (S1 and S2): "+S1.equalsIgnoreCase(S3));

		System.out.println("\n isEmpty method (checking name ): "+emp.isEmpty());

		System.out.println("\n compareTo() method (S1 == S2): "+S1.compareTo(S2));

		System.out.println("\n compareTo() method (S1 > S2): "+S2.compareTo(S3));

		System.out.println("\n compareTo() method (S1 < S2): "+S3.compareTo(S2));

		System.out.println("\n compareToIgnoreCase() method (S1 == S2): "+S3.compareToIgnoreCase(S2));

		System.out.println("\n concate() method : "+S1.concat(S4));

		System.out.println("\n join() method  Use of space between two strings : "+String.join(" ",S1,S4));

		System.out.println("\n subSequence() method :  "+name.subSequence(11,30));

		
		System.out.println("\n replace() method : "+S.replace("is","was"));

		System.out.println("\n replaceFirst() method : "+S.replaceFirst("is","was"));

		System.out.println("\n replaceAll() method : "+S.replaceAll("is","was"));

		System.out.println("\n replaceAll(using regular expression .)() method : "+S.replaceAll("is(.)","was"));

		System.out.println("\n replaceAll(using regular expression *)() method : "+S.replaceAll("is(.*)","was"));

		System.out.println("\n Initial string : "+name+"\n Length of the string : "+name.length()+"\n Is the string empty (T/F) : "+name.isEmpty()+"\nAfter removing spaces the string becomes: "+name.trim());

		System.out.println("\n use of substring(int begin)method : "+ S.substring(3));

		System.out.println("\n use of substring(int begin, int end) method :"+S.substring(3,10));

		System.out.println("\n indexOf method for first occurence  :"+S1.indexOf('i'));

		System.out.println("\n indexOf method for last occurence  :"+S1.lastIndexOf('i'));

		System.out.println("\n toUpperCase() method: "+S4.toUpperCase());

		System.out.println("\n toLowerCase() method: "+S3.toLowerCase());

		/* If i only want the no of characters in the string then  trim method will
		not be useful because it only trims the starting and ending spaces of a string not the middle one.*/
		System.out.println("After trimming the length becomes : "+name.trim().length());

        try
        {
			String nullstring = null;
			int i = nullstring.length();
        }
        catch (Exception e)
        {
			System.out.println("\n----------------------------------------------\n\n The line 'String nullstring = null'   will create a variable which is storing null. \n hence we are not able to calculate the length of the string.;");
       }

	}
}
 