# Codeforcescpp-112A
#include<bits/stdc++.h>
 
using namespace std;
 
int main(){
  string s1,s2;
  cin >> s1;
  cin >> s2;
  transform(s1.begin(), s1.end(), s1.begin(), ::tolower);
  transform(s2.begin(), s2.end(), s2.begin(), ::tolower);
  char str1[s1.length()+1];
  char str2[s1.length()+1];
  strcpy(str1,s1.c_str());
  strcpy(str2,s2.c_str());
  int n = strcmp(str1,str2);
  if(n > 0){
    cout << 1;
  }
  else if(n < 0){
    cout << -1;
  }
  else{
    cout << 0;
  }
  return 0;
}
