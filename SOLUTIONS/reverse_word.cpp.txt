#include<bits/stdc++.h>
using namespace std;
string reverseString(string & s){

    reverse(s.begin(),s.end());

    string res="",ans="";
    for(int i=0;i<(int)s.size();i++){
        if(s[i]!=' ')
        {
        res+=s[i];
        }
        else
        {
            reverse(res.begin(),res.end());

            ans+=res;
            ans+=" ";
            res="";
        }

    }
                reverse(res.begin(),res.end());

            ans+=res;
            res="";
                return ans;
}
int main(){
    string s;
        getline(cin,s);
    cout<<reverseString(s);
    return 0;
}
