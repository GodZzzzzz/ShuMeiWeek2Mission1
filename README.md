数媒-Android第二次作业

备注：因为本周过生日，所以时间非常匆忙，本次实验室作业可能存在许多不足之处望学长、老师指正；
由于下载的git文件上传器上传文件时有问题，因此现将代码复制到readme上
package week2;

import java.util.*;

public class mission1<T,t>
{
private T Zheng;
private t FuDian;

public mission1(T a,t b)
{
	Zheng=a;
	FuDian=b;
}
public String Shuchu()
{
return "整型数是："+Zheng+"浮点数是："+FuDian;
}


public T getZheng()
{
	return Zheng;
}

public void setZheng(T zheng)
{
	Zheng = zheng;
}

public void setFuDian(t fuDian)
{
	FuDian = fuDian;
}

public t getFuDian()
{
	return FuDian;
}



}
public static void main(String[] args) 
	{
		mission1<Integer,Float> num=new mission1<>(17,3.14f);
		
		
		List nums=new ArrayList();
		nums.add(num);
		
		for(int i=0;i<nums.size();i++)
		{
			mission1 d=(mission1)nums.get(i);
			System.out.println(d.Shuchu());
		}


	}




在本次作业中，我先学习了ArrayList类，在此过程中我了解到了
1、ArrayList与Array数组的区别，一个是用来储存数字一个是用来储存对象；
2、相比于数组，使用ArrayList的优势在于其不受长度大小影响，不许考虑储存问题
3、ArrayList可以对数据方便的添加、插入和移除。
4、学习了各种基本数据类型的封装类
而在此之后，我学习了泛型，泛型顾名思义就是规范数据类型（虽然两个fan字不一样但是应该可以这样理解吧，而且我也不知道为啥大多数网课上都说这个没有多大用处），泛型规定了类中使用的数据类型，并不允许使用除规定类型以外的数据类型。在学习泛型的网课当中我还学到了快速封装数据的快捷键：alt+shift+s。
