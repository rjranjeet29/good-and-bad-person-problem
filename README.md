#include <iostream>
using namespace std;

int main(){
   
   
   
   int T;
   cin>>T;
   while(T--){
    
    
    int n;
    cin>>n;
    int k;
    cin>>k;
    string s;
    cin>>s;
    int cap=0;
    int small=0;
    
    for(int i=0;i<n;i++){
        
        char x=s[i]; 
        int p =int(x);
        
        if(p>=65 && p<=90)
            cap++;
        else
            small++;
        
    }
    
    if(cap==small){
        if(k>=cap)
        cout<<"both"<<endl;
        else if(k<cap)
            cout<<"none"<<endl;
        
        
    }
    else if(small>cap)
    {
        if(k>=small)
            cout<<"both"<<endl;
        else if(k<cap)
            cout<<"none"<<endl;
            else
            cout<<"chef"<<endl;
    
        
    }
    else if(cap>small){
        if(k>=cap)
            cout<<"both"<<endl;
        else if(k<small)
            cout<<"none"<<endl;
            else
            cout<<"brother"<<endl;
        
    }
   }
}

