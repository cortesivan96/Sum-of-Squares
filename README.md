///# Sum-of-Squares
////Quiz 8 TC101

#include <iostream>
#include <vector>
#include <cmath>
using namespace std;

int sumsquares_list(){
  cout<< "Write Numbers and I Will Sum Their Squares (when yo want to stop, type -1)"<<endl;
  vector<int> num;
  int x, i;
  cin >> x;

  while(x != -1){
    num.push_back(x);
    cin >> x;
  }
int sum=0;
  for(i=0; i < num.size(); i++){
    sum = sum + pow(num[i],2);
  }
  cout<< "the result is: "<< sum << endl;

}
int main(){
  sumsquares_list();
  return 0;
}
