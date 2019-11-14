# laowang
# 计G191 2019322169 王智民
实验四 字符串实验

## 实验目的
---
掌握字符串String及其方法的使用
掌握异常处理结构
业务要求
内容：利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。达到如下功能：

1.	每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
2.	允许提供输入参数，统计古诗中某个字或词出现的次数
3.	考虑操作中可能出现的异常，在程序中设计异常处理程序

输入：汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行<未完，待续>
输出：
汉皇重色思倾国，御宇多年求不得。
杨家有女初长成，养在深闺人未识。
天生丽质难自弃，一朝选在君王侧。
回眸一笑百媚生，六宫粉黛无颜色。
春寒赐浴华清池，温泉水滑洗凝脂。
侍儿扶起娇无力，始是新承恩泽时。
云鬓花颜金步摇，芙蓉帐暖度春宵。
春宵苦短日高起，从此君王不早朝。
…………

注意： 输入的内容，利用main方法中的args数组传递
package hhh;
```Java
import java.util.Scanner;

public class Main {
	public static void main(String[] args) {
		try {
		
         String contxet = "汉皇重色思倾国御宇多年求不得杨家有女初长成养在深闺人未识天生丽质难自弃一朝选在君王侧回眸一笑百媚生六宫粉黛无颜色春寒赐浴华清池温泉水滑洗凝脂侍儿扶起娇无力始是新承恩泽时云鬓花颜金步摇芙蓉帐暖度春宵春宵苦短日高起从此君王不早朝承欢侍宴无闲暇春从春游夜专夜后宫佳丽三千人三千宠爱在一身金屋妆成娇侍夜玉楼宴罢醉和春姊妹弟兄皆列士可怜光采生门户遂令天下父母心不重生男重生女骊宫高处入青云仙乐风飘处处闻缓歌慢舞凝丝竹尽日君王看不足渔阳鼙鼓动地来惊破霓裳羽衣曲九重城阙烟尘生千乘万骑西南行";
         Scanner sc;
         char[] text = contxet.toCharArray();
         String text2;
         char text3;
         int count=1;
         int k=0;
         for (int i = 0; i < contxet.length(); i++) {
             System.out.print(text[i]);
             if (i % 7 == 6) {
                 if (count % 2 == 1) {
                     System.out.print("，");
                 } else {
                     System.out.print("。");
                     System.out.println("");
                 }
                 count += 1;
             }
         }
         System.out.println("");
         System.out.println("请输入你的文本：");
         
         
         sc = new Scanner(System.in);
         text2 = sc.next(); 
         text3=text2.charAt(0);
         sc = new Scanner(System.in);
         text2 = sc.next(); 
         text3=text2.charAt(0);
         for (int j = 0; j < contxet.length(); j++) {
        	 if (text3==text[j]) {
				k=k+1;
			}
        	 
		}
         System.out.println("出现次数："+k);
	
	
	} catch (Exception e) {
        e.printStackTrace();
    }
	}
         for (int j = 0; j < contxet.length(); j++) {
        	 if (text3==text[j]) {
				k=k+1;
			}
        	 
		}
         System.out.println("出现次数："+k);
	
	
	} catch (Exception e) {
        e.printStackTrace();
    }
	}
}
	
	} catch (Exception e) {
        e.printStackTrace();
    }
	}
         for (int j = 0; j < contxet.length(); j++) {
        	 if (text3==text[j]) {
				k=k+1;
			}
        	 
	}
		}
         System.out.println("出现次数："+k);
	
	
	} catch (Exception e) {
        e.printStackTrace();
    }
}
```
# 
