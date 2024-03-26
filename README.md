public class InitArray {
    public static void main(String[] args) {
        System.out.println("These are unmanipulated values");
       //Init the array
        //There will be 10 elements in this array
        //the elements will be ZERO through NINE
        int[] array = new int [10];

        //Loop through the array and print the values
        for(int counter = 0; counter < array.length; counter++){
            //The initial value of the array is 0
            //Condition of the for loop is for it to continue for as long as the counter is less that the array length
            //counter++ --> increment the couunter (until the condition of the for loop is false)
            
            System.out.printf("%5d%8d%n", counter, array[counter]);
            //output the array values
            //%5d --> print 5 spaces, then a decimal number
            //%8d --> print 8 spaces, then a decimal number
            //%n --> print a new line
            
            //This output of the array values will repeat since it is inside the 'for' loop
            //each time the counter increments --> print --> increment --> print
            
            //%5d%8d%n--> gives 5 spaces for decimal integers then 8 spaces
        }//End: for

        //Taking 2 array values and manipulating them and turning them into different values
        
        array[0] =123562;
        array[5] =923212;

        int sum = 0;

        //There's NO GUARANTEE of order
        //is gurantee it will go through all of them, but might start at 9th element, etc...
        //cannot manipulate array elements in a for 'each'

        //called a 'for each'
        for(int someElementInTheArray : array){
            sum += someElementInTheArray + 2;
        }//End: for
        //going to go through each element of the array

        
        System.out.println("*****************************");
        System.out.println("*****************************");
        System.out.println("*****************************");

        System.out.println("These are manupulated values.");

        //Print header row
        System.out.printf("%s%8s%n", "Index", "Value");
        //%8s --> adds 8 spaces
        //%-8s- dash will left align, if you dont have the dash it will right align

        //Loop through the aray and print the values
        for(int counter = 0; counter < array.length; counter++){
            System.out.printf("%5d%8d%n", counter, array[counter]);
        //gives 5 spaces for decimal integers
        }//End: for

    }//End: main
}//End: class
