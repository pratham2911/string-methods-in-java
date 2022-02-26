# string-methods-in-java
import java.nio.charset.StandardCharsets;
import java.sql.SQLOutput;
import java.util.Arrays;
import java.util.Locale;

public class String_methods {
    public static void main(String[] args) {
        System.out.println();
        System.out.println("******Stirng Method******");
        System.out.println();
        String s = " hello ";
        System.out.println("s.length() :" +s.length());//7
        System.out.println("s.contains(\"he\") :" +s.contains("he"));//true
        System.out.println("s.isEmpty : "+ s.isEmpty());//false
        System.out.println("s.toUpperCase() : " +s.toUpperCase());//HELLO
        System.out.println("s.startsWith(\"h\"): "  +s.startsWith("h"));//false
        System.out.println("s.endsWith(\" \"):" +s.endsWith(" "));//true
        System.out.println("s.replace(\"LL\"):"+ s.replace("ll","LL"));// heLLo
        System.out.println("s.trim():"+ s.trim());//hello
        System.out.println("s.substring(0,3):" + s.substring(0,3));//he
        System.out.println("Arrays.toString(s.getBytes()):" + Arrays.toString(s.getBytes()));//[32, 104, 101, 108, 108, 111, 32]
        System.out.println("Arrays.toString(s.toCharArray()):" + Arrays.toString(s.toCharArray()));//[ , h, e, l, l, o,  ]
        System.out.println("s.charAt():" + s.charAt(2));//e
        System.out.println("Arrays.toString(s.split(\"e\")): "+Arrays.toString(s.split("e")));//[ h, llo ]
        System.out.println(s);// hello
        System.out.println();
        System.out.println("*********Strings Comparison********");
        System.out.println();
        String s2 = " hello ";
        System.out.println("s == s2:" +(s==s2));//true
        String s3 = new String(" hello ");
        System.out.println("s == s3: "+(s ==s3));//false
        System.out.println("s.equals(s3):" + s.equals(s3));//true
        System.out.println("s ==s3.intern() :" + (s ==s3.intern()));//true
        String firstname = "Pratham";
        String firstname2 = "pratham";
        System.out.println("firstname.equals(firstname2):" +firstname.equals(firstname2));//false
        System.out.println("firstname.equalsIgnoreCase(firstname2):" + firstname.equalsIgnoreCase(firstname2));//true
    }
}
