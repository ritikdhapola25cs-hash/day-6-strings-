# day-6-strings-
Day 6 of the c++ programming in the summer training camp 
//this is the program of the counting the no of element in the sting 


#include<iostream>
using namespace std;
int countstring(string s){
    int count=0;
    for(int i=0;i<s.length();i++){
        count++;
    }
    return count;
}
int main(){
    string st="hello sir ";
    cout<<"the number of words in the sting is "<<countstring(st)<<endl;
    return 0;
}


//this is the program of the counting the no of the vowel in the sting 

#include<iostream>
using namespace std;
int countstring(string s){
    int count=0;
    for(int i=0;i<s.length();i++){
        if(s[i]=='a'||s[i]=='e'||s[i]=='i'||s[i]=='o'||s[i]=='u'){
        count++;}
    }
    return count;
}
int main(){
    string st="hello sir ";
    cout<<"the number of words in the sting is "<<countstring(st)<<endl;
    return 0;
}


//this the program of the reversing the sting 


#include<iostream>
#include<algorithm>
using namespace std;
string reversestring(string s){
    int n=s.length();
    string ans=" ";
    reverse(s.begin(),s.end());
    return s;
}
int main(){
    string st="jai shree ram ";
    cout<<"REVERSING"<<endl;
    cout<<reversestring(st);
    return 0;
}

//this is the program of the uppercase and the lowercase conversion

#include<iostream>
using namespace std;
string uppperlower(string s){
    for(int i=0;i<s.length();i++){
    if(toupper(s[i])!=(s[i])){
        s[i]=toupper(s[i]);
    }
    else s[i]=tolower(s[i]);}
    return s;
}
int main(){
    string st="HellO My NAme IS PEter";
    cout<<uppperlower(st);
    return 0;
}



//this is the program of the valid palindrome in the case of the string

#include<iostream>
using namespace std;
bool validpallindrome(string s){
    int n=s.length();
    int st=0,end=n-1;
    while(st<end){
        if(tolower(s[st])!=tolower(s[end])){
            return false;
        }
        st++;end--;
        
    }
    return true;
}
int main(){
    string s="RaceCar";
    if(validpallindrome(s)){
        cout<<" this is the valid pallindrome "<<endl;
    }
    else
    cout<<" this is not the valid pallindrome "<<endl;
    return 0;
}
