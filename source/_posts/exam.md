title: 計算機程式
author: John Doe
date: 2024-01-12 01:23:26
tags:
---
```
#include<cstdlib>
double
char 
int
```

volume 
```
class Volume
{ 
  public:
     Volume(int l, int w, int h);
  private:
      int Vlen;
      int Vwid;
      int Vhei;
};

Volume::Volume(int l, int w, int h): Vlen(l), Vwid(w), Vhei(h)
{
    cout << l * w * h << endl;
}
int main(){
  Volume H(1, 1, 1);
  H = Volume(2, 3, 5);
}
```
#### 四種表達方式
* 普通

* function
* struct 
```
struct AREA
{ int len;
  int wid;
};
int main()
{
	AREA R;
	int area;
	cin >> R.len >> R.wid;
	area=R.len*R.wid;
	cout << area << endl; 
```

* class 

  ```
  class AREA
  { 
    public:
       int len;
       int wid;
       int mult();
  };

  int AREA::mult()
  {
      return len*wid;
  } 

  int main()
  {
      AREA R;
      int area;
      cin >> R.len >> R.wid;
      area=R.mult();
      cout << area << endl; 
   }
  ```

#### 文件更改

``` cpp
#include <fstream>

// 創建對象
ifstream 讀取
ofstream 將更改的文件


.open(...)  	//開啟文件  (若括號中加入 ,ios::app ，不會覆蓋) 
.close() 		//關閉讀取文件
.fail()   		//讀取失敗    exit(1); 離開
.get(next) 		//讀取下一個字符
.eof() 			//查文件流是否已經到達了文件的結尾（End of File，EOF）
```