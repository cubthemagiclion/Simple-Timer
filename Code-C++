#include <iostream>
#include <ctime>
#include <list>
using namespace std;

void func1(list<int> l){
}

void func2(const list<int>& l){
}

class Timer{
  double start;
public:
  Timer():start(clock();{}
  void reset(){start=clock();}
  double elapsed(){return (clock() - start)/CLOCKS_PER_SEC;}
};

int main(){
  Timer t;
  list<int> l;
  for(int i=0;i<10000000;i++)
    l.push_back(i);
  double elapsed;
  cout<<"List created<<endl;
  t.reset();
  func1(1);
  elapsed = t.elapsed();
  cout<<"With size"<<l.size()<<" func1 took "<<elapsed<<" seconds "<<endl;
  
  t.reset();
  func2(1);
  elapsed = t.elapsed();
  cout<<"With size"<<l.size()<<" func2 took "<<elapsed<<" seconds "<<endl;
