## Welcome to sdyin's GitHub Pages

You can use the [editor on GitHub](https://github.com/sdyin/sdyin.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

文档笔记

```markdown
二叉树遍历：
-前序遍历：先输出当前结点的数据，再依次遍历输出左结点和右结点
-中序遍历：先遍历输出左结点，再输出当前结点的数据，再遍历输出右结点
-后序遍历：先遍历输出左结点，再遍历输出右结点，最后输出当前结点的数据

# Header 1
## Header 2
### Header 3

广度优先搜索(BFS):
    从根节点出发，在横向遍历二叉树层段节点的基础上纵向遍历二叉树的层次。
    广度优先遍历图的方式，是以一种类似波纹扩散的方式进行的，不断放大辐射半径，进而覆盖整张图。
    实现方式：
        1.选择起始顶点放入队列，并标记为已访问；
        2.当队列不为空时，从队列中取出顶点作为目标顶点，将目标顶点的所有相邻且未被访问过的顶点放入队列，并标记为已访问；
        3.重复执行步骤 2。

深度优先搜索(DFS):
    回溯思想,适合用递归实现。
    从根节点出发，沿着左子树方向进行纵向遍历，直到找到叶子节点为止。
    然后回溯到前一个节点，进行右子树节点的遍历，直到遍历完所有可达节点为止
    实现方式：
        1.选择起始顶点入栈，并标记为已访问；
        2.当栈不为空时，选择栈顶元素作为目标顶点，若目标顶点存在未访问状态的相邻顶点，则将该相邻顶点入栈，并标记为已访问；若不存在未访问状态的相邻顶点，则执行出栈操作；
        3.重复执行步骤 2。
        

动态规划(TODO):


spring事务：
    1.获取当前事务名：TransactionSynchronizationManager.getCurrentTransactionName()
    2.同一类中：a方法调用b方法均是同一事务，除非使用代理类调用b方法，且申明b方法是事务传播属性新建事务。
        获取当前类代理对象方式
        ①：<!-- 开启暴露Aop代理到ThreadLocal支持  -->  
           <aop:aspectj-autoproxy expose-proxy="true"/>  
           ((类名) AopContext.currentProxy()).方法();  

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sdyin/sdyin.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
