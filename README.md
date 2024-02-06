# UCAS_Ping
Selenium实现半自动化教评
23硕士生，寒假提前入组，没事可做开始琢磨爬虫，用上Selenium，便想着搞一个能够自动进行课程评价的工具，便有了这个repository。
为什么说是半自动化呢，识别验证码有点麻烦，这里就没再往下搞（还是因为懒）。
主要思路还是通过工具模拟我们点击、输入的操作，在打分和输入评价那里能省一点时间。
## 前期准备
- python>=3.11
- selenium
- Chrome Drive~~或者Edge Drive~~
### Selenium安装
```
pip install selenium
```
or
```
conda install selenium
```
### Chrome Drive
可通过该链接获取：
https://chromedriver.chromium.org/downloads 

~~### Edge Drive
可通过该链接获取：
https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/?form=MA13LH#downloads~~

## 使用
```
usage: ucas.py -u <email> -p <password> -o <confirmation>

                #############################
                # #   #   ###   ###    #### #
                # #   #  #     #   #  #     #
                # #   #  #     #####   ###  #
                # #   #  #     #   #      # #
                #  ###    ###  #   #  ####  #
                #############################


options:
  -h, --help            show this help message and exit
  -v, --version         show program's version number and exit
  -u USERNAME, --username USERNAME
                        邮箱
  -p PASSWORD, --password PASSWORD
                        密码
  -o OK, --ok OK        任意字符串确认

V wo wu shi, I want to eat crazy Thursday KFC
```
结果：

![image](https://github.com/yf8578/UCAS_Ping/assets/71922803/4e3c9092-d554-4bf3-84cc-78b08dad56cd)

