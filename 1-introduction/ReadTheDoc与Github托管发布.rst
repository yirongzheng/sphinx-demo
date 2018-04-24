==================================
通过ReadTheDocs与Github托管发布
==================================

如果用sphinx把自己的文档发布成静态网页或pdf当然都很好，但不方便的地方在于，如果我们需要对文档进行修改或是增减内容，
那么我们每做一次修改，都需要进到index.rst界面添加一次目录，然后再用cmd执行一次-build命令，这样显然非常麻烦，
所以我们在这里再介绍一款工具，可以轻松帮助我们对文档进行发布。

1. 进入https://readthedocs.org/ 并注册一个账号；
2. 在自己的Github上新建一个sphinx项目repo；
2. 将ReadTheDocs（以下简称RTD）账号与自己的Github账号相关联；
4. 在RTD上新建一个project并将其与Github上的sphinx repo相关联；
5. 下载Github Desktop桌面版，登陆，然后把sphinx repo clone到本地；
6. 打开sphinx repo本地仓库所在文件夹，把source文件夹中的conf.py index.rst 以及自己建立的用于写rst文档的文件夹放到本地仓库然后再push；
7. 之后每次需要对内容进行增删改等操作时，直接在本地仓库中进行修改然后再push上去就好啦~

当在线repo中有任何变动时，RTD都能检测到并帮你发布，妈妈再也不用担心我每次发布都要-build一次啦~
