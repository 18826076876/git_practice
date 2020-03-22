﻿------------------------------Program_handling_data-----------------------------

此程序用于处理从MTS机器实现材性试验得到的的txt数据，使用该程序可批量处理txt文件数据，
智能判断各点斜率，帮助排除误差点，处理拉压试验的卸载后多余数据点，从而直接生成报告或
论文中所需的图片。

----------------------------------使用步骤------------------------------------------
小程序主要分为三个文件，”main"，“func”，“deal”，运行时中需把三个文件放在同个
目录下并打开“main”文件运行即可。

一，使用前请在本机电脑中安装好所需的第三方库文件：matplotlib，numpty。
    安装时请学确认本机为何种操作系统和python版本，然后可在网上查询不同操作系统
    安装python第三方库的使用教程。本示例为win10系统，使用python3.7，如先用谷歌
    搜索“matplotlib pypi”，然后下载whl文件，再使用终端进入下载好的该文件目录下，
    使用命令“python -m pip installl user "该whl后缀名文件的全名称" ”；

二，安装好第三方库后，请打开main文件，在使用Load函数时，需传递两个变量实参，其中
    一个为数据所在文件夹名称（源代码种对应为“data”），建议该文件夹处在与代码
    同个目录下；另外一直是实参代表生成最终图片所指的文件夹名称，默认填入image即可，
    小程序会自动创建该文件并存放图片；

三，func文件封装了处理数据和画图所需的两个函数，如需自行开发的可单独提取这两个函数，
    deal文件中封装了三个类，分别时读取数据所需的“Load”，筛选数据所需的“Del”,和
    求解斜率所用的“KK”类，使用者可使用单独使用该类。

---------------------------------------------------------------------------------------
使用过程若有任何问题均可在我的Github账号上留言，或者联系我邮箱“969358865@qq.com”


