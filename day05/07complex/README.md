# 双目操作符重载

## 运算类双目操作符：+、-、*、/等

* 左右操作数均可为左值或右值
* 表达式的值为右值
* 成员函数形式
  ```
  class LEFT {
  	const RESULT operator#(const RIGHT& right) const { ... }
  };
  ```
* 全局函数形式
  ```
  const RESULT operator#(const LEFT& left, const RIGHT& right) { ... }
  ```

## 友元

* 可以通过`friend`关键字把 一个全局函数、另一个类的成员函数或者另一个类整体，声明为某个类的友元
* 友元拥有访问授权类任何非公有成员的特权
* 友元声明可以出现在授权类的公有、私有或者保护等任何区域，且不受范围控制限定符的约束
* 友元不是成员，其作用域并不隶属于授权类，也不拥有授权类类型的this指针
* 操作符函数常被声明为其参数类型的友元









