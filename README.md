# Character-Arrays
This program shows character arrays: how to fill them and sort them.

public class CharacterArrays {
    public static void main(String [] arg) {
        // Create two methods, one creating a character array and another sorting it. Call both from main
        char [] arr=fillingArray();
        for(int i=0;i<arr.length;i++){
            System.out.print(arr[i] + " ");
        }
        System.out.println();
        sortingArray(arr);
        for(int i=0; i<arr.length;i++){
            System.out.print(arr[i] + " ");
        }



    }
    public static char [] fillingArray () {
        char[] arr= {'m', 'a', 'r', 'i','a', 'm'};
        return arr;

    }
    public static void sortingArray(char[] arr) {
        for(int i=0;i<arr.length;i++) {
            for(int j=i+1;j<arr.length;j++) {
                if(arr[i]>arr[j]) {
                    char temp=arr[i];
                    arr[i]=arr[j];
                    arr[j]=temp;
                }
            }
        }
    }
}
