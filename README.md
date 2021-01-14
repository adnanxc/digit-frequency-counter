#include <iostream>
using namespace std;


int main(){
    int x;
    cout << "Enter a number: ";
    cin >> x;
    int ctr , temp , d;
    for(int i=0; i<=9; i++){
        ctr = 0;
        for(int j=x; j>0; j=j/10){
            d = j%10;
            if(d==i){
                ctr++;
            }
        }
        cout << "The frequency of " << i << " is = " << ctr << endl;

    }

    return 0;
}
