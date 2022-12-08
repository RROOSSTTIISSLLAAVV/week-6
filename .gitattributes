#include <iostream>
#include <math.h>

using namespace std;

int length(int n) {
    if (n == 0) return 1;
    int l = 0;
    while(n) {
        l++;
        n /= 10;
        }
    return l;
    }

int main()
{
    int n;
    cin >> n;
    int len = length(n);
    int arr[length(n)];
    
    if (len==1) cout << n << endl;
    
    else {
        for (int i=0; i<len; i++){
            arr[i] = n/pow(10,(length(n)-1));
            
            n -= int(n/pow(10,(length(n)-1))) * pow(10,(length(n)-1));
            
        }

        n = arr[0];
        arr[0] = arr[len-1];
        arr[len-1] = n;
        n = 0;
        
        for (int i=0; i<len; i++){
            n += arr[len-1-i]*pow(10,i);
        }
        
        cout << n;
    }
}
