public class InitArray {
    public static void main(String[] args) {

       //Init the array
        //There will be 10 elements in this arry
        //the elements will be ZERO through NINE
        int[] array = new int [10];

        //Print header row
        System.out.printf("%s%8s%n", "Index", "Value");
        //%8s --> adds 8 spaces
        //%-8s- dash will left align, if you dont have the dash it will right align

        //Loop through the aray and print the values
        for(int counter = 0; counter < array.length; counter++){
            System.out.printf("%5d%8%n", counter, array[counter]);
        //gives 5 spaces for decimal intergers
        }//End: for
    }//End: main
}//End: class
