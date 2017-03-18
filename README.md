# BubbleSort

/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package bublesort;

import java.util.Arrays;

/**
 *
 * @author Тарас Вікторович
 */
public class BubleSort {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {

        int array[] = {2, 3, 4, 4, 10, 4, 5, 1, 6, 9};
        boolean swapped = true;
        int z = 0;
        while (swapped) {
            swapped = false;
            for (int i = 0; i < array.length - 1 - z; i++) {
                if (array[i] > array[i + 1]) {
                    int a = array[i];
                    array[i] = array[i + 1];
                    array[i + 1] = a;
                    swapped = true;
               }
 
            }
            z++;
        }
        System.out.println(Arrays.toString(array));
    }

}
