# Mission5

public class Mission5 
{

    public static void mission() 
    {
        
        Integer x = 3, y = 5, temp1, temp2;
        List<Integer> input = new List<Integer> {12, 20, 30, 17}; //declare the numbers in the list
        	System.debug(input); // Output to check if the list we have is correct
        
        for(Integer num : input) 
        {
            temp1 = Math.mod(num, x); //Setting the remainder for 3
            temp2 = Math.mod(num, y); //Setting the remainder for 5
            
            if (temp1 == 0 && temp2 != 0) 
            {
                System.debug(num + ' is a multiple of 3. Displaying output: Ding');
            }
            
            if (temp1 != 0 && temp2 == 0) 
            {
                System.debug(num + ' is a multiple of 5. Displaying output: Dong');
            }
            
            if (temp1 == 0 && temp2 == 0) 
            {
                System.debug('Input numbers are a multiple of 3 & 5. Displaying output: DingDong');
            } 
            
            if (temp1 != 0 && temp2 != 0) 
            {
                System.debug('Input numbers are not a multiple of 3 & 5. Displaying output: 17');
            } 
        }
    }
}
