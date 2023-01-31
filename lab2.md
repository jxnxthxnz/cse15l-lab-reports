**Part 1**
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {

    String x = "";

    public String handleRequest(URI url) {
        if (url.getPath().equals("/")) {
            return String.format(x);
        } else {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {
                    for (int ii = 1; ii < parameters.length; ii++) {
                        x += parameters[ii] + " ";
                    }
                    x += "\n";
                    return String.format(x);
                }
            }
        }
        return "404 Not Found!";
    }
}

class SearchEngine {
    public static void main(String[] args) throws IOException {
        if (args.length == 0) {
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
![Image](AddWord1.png)
![Image](AddWord2.png)
-In both screeenshots, the method handRequest was called\
-In both screeenshots, the only relevant argument is `URI url` which is the url we enter. The relevant fields include the path (equal to `/add-message`), the string to return (intially equal to ""), and the query (equal to `s=word`, word can change based on what we enter).
-In pic 1, the query is equal to `s=Bye`, and the string is equal to `"Bye" + "\n"` In pic 2, the query is equal to `s=How Are You Today`, and the string is equal to `"Bye" + "\n" + "How Are You Today" + "\n`

**Part 2**
```
@Test 
  public void testReverseBig() {
    int[] input = {1, 2, 3, 4};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[] {4, 3, 2, 1}, input);
  }
```
``` 
@Test 
  public void testReverseSame() {
    int[] input = {1, 2, 2, 1};
    ArrayExamples.reverseInPlace(input);
    assertArrayEquals(new int[] {1, 2, 2, 1}, input);
  } 
```
![Image](ReverseBig.png)
![Image](ReverseSame.png)
```
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length / 2; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
```
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length / 2; i += 1) {
      int x = arr[arr.length - i - 1];
      arr[arr.length - i - 1] = arr[i];
      arr[i] = x;
    }
  }
```
The initial code didn't work because it did not replace any of the values in the second half of the array. In my fixed code, as the for loop traverses the array, both halves of the array have their values replaced with the correct reverse values.\
**Part 3**\
In week 2, I learned about urls and more specifically, what the path and the query are and how to identify them in a url. In week 3, I learned about JUnit as a way to test my programs. Typically, I would have to handwrite my expected results and compare them to the programs which was bothersome at times. With JUnit, it makes the debugging process much more efficient and effective. 
