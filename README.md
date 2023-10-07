# reverseofarray-Github
#include<bits/stdc++.h>
using namespace std;

int main() {
    int arr[] = {1, 2, 3, 4, 5};
    int start = 0;
    int end = sizeof(arr)/sizeof(arr[0]);  

    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;

        start++;
        end--;
    }

    for (int i = 1; i <=sizeof(arr)/sizeof(arr[0]); i++) {
        cout << arr[i] << " ";
    }
       
    return 0;
}












