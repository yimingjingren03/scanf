# scanf
scanf+while的用法，假（0）和真（非0）的判定，
/*  格式：scanf("<格式化字符串>",<地址列表>);
 *  
 *  scanf的返回是有值的
 *  当正确输入（参数相对）之后，返回的值为正数
 *  当错误输入之后（参数不匹配），返回的值为 0 
 *  当输入的是Ctrl+z时，返回的值是 -1
 *  
 *  while的判断条件 
 *  非0继续循环 
 *  当等于0时，中断循环
 *  
 *  while（~scanf（“%d”，&a））
 *  window当输入ctrl+z时停止输入
 *  Linus/Unix输入Ctrl+d停止输入
 *  -1用二进制表示11111111
 *  ~（-1）为0000000，条件便为0，
 *  while（0）便停止输入
 */
 #include<stdio.h>
  int main()
  {
  int a,b;
  
  while(~scanf("%d%d",&a,&b))
  printf("%d",a+b);
  
  return 0;
  }
