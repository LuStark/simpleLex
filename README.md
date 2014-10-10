regex-engine(demo)
-------------------------
1.  regex-engine目前处于测试状态，对输入的正则表达式以及给定文本进行匹配，
    识别成功的子串以空格隔开。
    
2.  目前能匹配基本正则表达式，以及两种扩展表达式:正反向预查
     而且我相信只要能精简数据结构，以后可以更容易引入更多功能：
     例如：重复，匿名捕获，任意字符识别等等。

3.  使用示例:  
    匹配部分前后用一个空格隔开  
    1. 闭包  
        输入正则表达式:  a*  
        输入正文: vfdbvjekbnjwkaabrbaaaabrebe  
        
        显示输出: vfdbvjekbnjwk aa brb aaaa brebe  
    
    2. 正向预查  
        输入正则表达式:  Windows(?=7|8)  
        输入正则表达式:  vvnrekbwnkjcxnvveancvehwvuirwehrrbgvWindowsvvujenvWindows7vavnkjWindows8?bnfl  
        
        显示输出: vvnrekbwnkjcxnvveancvehwvuirwehrrbgvWindowsvvujenv Windows7 vavnkj Windows8 ?bnfl  
    
