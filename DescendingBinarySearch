    /*Finds index of element in a sorted descending order array rather than ascending sorted if present
    * else return -1*/
    private static int descendingSortedBinarySearch (int descendingSortedArray[],int startIndex,int stopIndex,int elementToFind){

        int mid;
        if (stopIndex>=startIndex){
            mid = startIndex + (stopIndex -startIndex)/2;

            /*if element is present in middle itself*/
            if (descendingSortedArray[mid] == elementToFind){
                System.out.println("***Mid : "+mid);    //Uncomment to DEBUG
                return mid;
            }

            /*If element is smaller than mid, then it can only be present in right sub-array*/
            if (descendingSortedArray[mid] > elementToFind){
                System.out.println("***Return right ");    //Uncomment to DEBUG
                return descendingSortedBinarySearch(descendingSortedArray,mid+1,stopIndex,elementToFind);
            }

            /*Else element can only be present in left sub-array*/
            System.out.println("***Return left ");    //Uncomment to DEBUG
            return descendingSortedBinarySearch(descendingSortedArray,startIndex,mid-1,elementToFind);
        }

        /*We reach here only if element was not found*/
        return -1;
    }
