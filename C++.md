<h4>The inherit system</h4>

```c++
class Father{
    
    public:
    	void func(){
            cout << show << endl;
        }
    private:
    	int  show = 10;
    protected:
    
};
class Son: public Father{
    private:
    	int show = 20;
   
};
int main(){
    Son son;
    son.func();//Here it actually print out 10.
}
```

SO apparently, inherit system in c++ uses the function and variable space in the base class.

If you want to use the private variables in Son class, but the function itself is in the Father class then define the function with variables.