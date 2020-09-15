助开发人员编写代码,提升质量、减少bug。如果大家分析一下我们bug原因的构成,...
提升反馈速度,减少重复工作,提高开发效率。开发人员实现某个功能或者修补了某个bug,...
保证最后的代码修改不会破坏之前代码的功能。项目越做越大,代码越来越多,...
让代码维护更容易。由于给代码写很多单元测试,相当于给代码加上了规格说明书,...
有助于改进代码质量和设计。





package li;
public class maopao {
    public static void main(String[] args) {
        int[] numbers=new int[]{1,5,8,2,3,9,4};
        int i,j;
        for(i=0;i<numbers.length-1;i++)
        {
            for(j=0;j<numbers.length-1-i;j++)
            {
                if(numbers[j]>numbers[j+1])
                {
                    int temp=numbers[j];
                    numbers[j]=numbers[j+1];
                    numbers[j+1]=temp;
                }
            }
        }
        System.out.println("排序后的结果是:");
        for(i=0;i<numbers.length;i++)
            System.out.print(numbers[i]+" ");
    }
}

package li;

import static org.junit.Assert.*;

import org.junit.Before;
import org.junit.Test;

public class maopaoTest {

	@Before
	public void setUp() throws Exception {
	}

	@Test
	public void testMain() {
		fail("Not yet implemented");
	}

}




