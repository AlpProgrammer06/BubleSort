```
package com.company;

public class Main {


    // 1  3  5  7  8
    public static void main(String[] args) {
        int[] dizi = new int[9];
        for (int i = 0; i < dizi.length; i++) {
            dizi[i] = (int) (Math.random()*10);
        }
        int temp;
        for (int i = 0; i < dizi.length; i++){
            System.out.print( dizi[i]);
        }

        // 1   2  3  5   8
        System.out.println();
        for (int i = 0; i < dizi.length - 1; i++) {.
            for (int j = 0; j < dizi.length - 1 - i; j++) {
                if (dizi[j] > dizi[j + 1]) {
                    temp = dizi[j];
                    dizi[j] = dizi[j + 1];
                    dizi[j + 1]=temp;
                }
            }

        }  for (int i = 0; i < dizi.length; i++) System.out.print(dizi[i]);

    }
}

```