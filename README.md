# Reverse-Sentence-In-place
```java
class Solution {
    public String reverseSentence(String sentence) {
        String[] arr = sentence.split(" ");
        String temp;
        int iStart = 0;
        int iEnd = arr.length - 1;
        while (iStart < iEnd) {
            temp = arr[iStart];
            arr[iStart] = arr[iEnd];
            arr[iEnd] = temp;
            iStart++;
            iEnd--;
        }
        return String.join(" ",arr);
    }
}
```
