# Road_genius
简单易上手的路线编辑网页
一个能无学习成本进行旅行路线规划的网页，搭载有通义千问智能体对路线进行评估
文件夹里：road_genius.html：未嵌入智能体的单机编辑网页
 <img width="665" height="428" alt="image" src="https://github.com/user-attachments/assets/1521d8bb-bc4c-4d04-a1fd-de6338ab3e87" />
Road_genius_promax.html：在自由编辑路径的前提下，可以利用通义千问模型自行识别用户编辑的路径，并给出分析结果，如果用户没有很好的绘制思路，还可以直接通过直接输入需求提问以获得路径规划方面的帮助。
<img width="865" height="546" alt="image" src="https://github.com/user-attachments/assets/fde8c620-8c0e-42d0-95b3-3e4cf417a343" />
Promax版本已上传至腾讯云生成网页，可通过网址：
http://192.144.142.60/o202301073017/road_genius_promax.html访问

以下为简要图文说明部分：
其实一开始想做这个网页是出于一个契机，国庆我打算自驾去甘南旅游，在制作前期攻略时，我发现通过PS等制图软件绘制路线图等不仅效率较低，并且对图像编辑能力有一定要求，一般突发奇想想要制作旅游攻略的同学都没法很好地利用这些专业的制图工具制作自己的行进攻略图。
<img width="732" height="594" alt="image" src="https://github.com/user-attachments/assets/d5a98fe6-ac0c-4040-84bd-a3af143dc530" />
于是，我想到用网页的形式，对绘制路线的功能进行特化，使其具备通过简单的操作就能绘制路线的功能，让热爱旅游的电脑小白们能够在对网站的操作有最基本的了解后，即刻上手，绘制自己的旅游攻略图。 
<img width="833" height="523" alt="image" src="https://github.com/user-attachments/assets/c7a18181-93f9-482f-a36b-40b0506ff71f" />
首先是画面的整体设置，相当于ps的画布设置，此处我针对出行的规划需求做了一定的特化，首先是网格，用户可以自行设置行列；比例尺的引入让用户能够根据自己行程的远近自行设定单个网格所代表的距离，更贴合每个人旅程远近的个性化需求。
<img width="543" height="448" alt="image" src="https://github.com/user-attachments/assets/933025cf-8a8a-4f5c-bf78-527dd515a1e7" />
随后是线路编辑器，用户能够进行调度的其实是画布中的点与线，点代表出行经过的重要节点，比如风景区、打卡地、住宿点等，每当用户打下一个点时，都可以填入自己计划旅行的实际到达位置，并写入备注，当然，我还提供了多种颜色以便区分。
<img width="865" height="643" alt="image" src="https://github.com/user-attachments/assets/c39d5802-643d-4400-9804-f82cb0ba96b0" />
除了点的编辑，线路也很重要，区别于点的完全填充，我对线路的表示做出了区分，用网格中心的圆表示，但是区别于节点，线路往往是连贯的一条线，这时候如果一个一个打点，效率就很低了，于是，我专门设置了线路模式，进入线路模式后，用户可以移动鼠标，从一个点把线路拖到另一个点。如果觉得还不够便利，我还设置了长按快捷键“Alt”，快速进入线路模式进行编辑，如果有绘制出错或是计划放弃线路，可以点击左侧的线路界面进行快速删除。
<img width="635" height="661" alt="image" src="https://github.com/user-attachments/assets/1f3fa004-6247-4e84-8ed6-8237574baeb6" />
<img width="865" height="444" alt="image" src="https://github.com/user-attachments/assets/db936508-9c94-440a-b07d-ecc2dd961b12" />
在完成了节点和线路的位置后，如果对整个规划还存在一定疑问，怎么办？这时，我们就可以求助接入的通义千问，点击分析，它会自动读取用户编辑好的线路并给出建议。
<img width="865" height="391" alt="image" src="https://github.com/user-attachments/assets/a176dc98-be72-4b33-b438-c3d3c326a2b8" />
可以看得出来，他会指出用户的路线存在绕路等不合理之处，方便用户进行改进（乱画的，结果被ai批评了）

