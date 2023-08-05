# InsertionSort
here is a code of InsertionSort in java.

import java.util.Arrays;
public class SortingInsertionSort {
    public static void InsertionSort(int array[]){
        for(int i=1;i<array.length;i++){
            int CurPos =i;
            int PrePos =i-1;
            while(PrePos>=0 && array[PrePos]> CurPos){
                array[PrePos+1] =array[PrePos];
                PrePos--;
            }
            array[PrePos+1] =CurPos;
        }

    }
    public static void printarray(int array[]) {
        for(int i=0;i<array.length;i++){
            System.out.print(array[i]+ " ");
        }
        System.out.println();
    }


    public static void main(String[] args) {
        int array[] ={5,4,2,1,3};
        InsertionSort(array);
        printarray(array);
    }
}
