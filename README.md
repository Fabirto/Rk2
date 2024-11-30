#include <string>
#include <map>
#include <iostream>

using namespace std;

map<char,int> lettersCount( string str) {
    map<char,int> letters;
    
    for (int i = 0; i < str.size(); i++) {
        auto c = str[i];
        letters[c]++;
}
 return letters;
}



int main() {
    
    string str = "aaajabbbvvv";
    map <char, int> ans = lettersCount(str);
 for (auto pos : ans) {
     cout <<pos.first << " " << pos.second << endl;
 }
 }
    
