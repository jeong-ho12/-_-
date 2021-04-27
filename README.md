-> #include<iostream> //헤더파일

using namespace std; 
/* 
#define _plus(a,b)(a+b)
#define _A 100   <-  //여기까지 전처리 선언문(컴파일 이전에 실행, ;가 안붙음)
void main()
{
    cout << "Hello world!" << endl;
     char a;
     a = 97;
     cout << a<< endl;
     double k=10.0;
     double n=11.0;
     cout<<_plus(k, n)<<endl;
     cout << _A;
     return;
}
*/

#define _PRE_TEST01 100
#define _PRE_TEST03
int main()
{
#ifdef _PRE_TEST02
    
    cout << "true" << endl;
#else
    cout << "false" << endl;
#endif
    cout << _PRE_TEST01 << endl;

#ifdef _PRE_TEST02
       cout << "true" << endl;
#endif
#ifndef _PRE_TEST02
    cout << "false" << endl;
#endif

    return true;
}
