# Check-if-the-string-contains-consecutive-letters-and-each-letter-occurs-exactly-once-in-cpp



```
#include<bits/stdc++.h>
using namespace std;
bool check(string s)
{
    sort(s.begin(),s.end());
for(int i=1;i<s.size();i++)
{
if(s[i]-s[i-1]!=1)
{
return false;
}
}
return true;
}
int main()
{
string s;
 cin>>s;
 if(check(s))
 {
 cout<<"YES"<<endl;
 }
 else
 {
 cout<<"No"<<endl;
 }
 return 0;
}
