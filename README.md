# Linux_learn_word_color
給予文字顏色

參考 : 
* https://stackoverflow.com/questions/5947742/how-to-change-the-output-color-of-echo-in-linux
* https://www.codegrepper.com/code-examples/shell/bash+echo+color

You can use these ANSI escape codes:

```Bash
Black        0;30     Dark Gray     1;30
Red          0;31     Light Red     1;31
Green        0;32     Light Green   1;32
Brown/Orange 0;33     Yellow        1;33
Blue         0;34     Light Blue    1;34
Purple       0;35     Light Purple  1;35
Cyan         0;36     Light Cyan    1;36
Light Gray   0;37     White         1;37
```
範例 : 

![image](https://user-images.githubusercontent.com/96226780/201520701-fd807863-df3a-4315-967b-b3b7f64bb8c4.png)

```Bash
RED='\033[0;31m'
NC='\033[0m' # No Color
echo -e "I ${RED}love${NC} Stack Overflow\n"

#echo -e "I \033[0;31mlove\033[0m Stack Overflow\n"
```
