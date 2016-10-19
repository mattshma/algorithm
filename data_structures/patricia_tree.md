# Patricia tree

Patricia tree在Linux中又被称为Radix tree，其将tire中只有一个孩子的节点与其父节点合并，这种能有效减少tire的高度。

具体实现的话，不同应用有各自不同的变种，比较常见的一种实现是将字符串或数字转化为相应bit位进行存储，根据radix分叉的不同可分为2叉radix树，4叉radix树,……。Linux中实现的是64叉Radix树，其用来存放pagecache相应信息。


## Reference
- [Radix tree](https://en.wikipedia.org/wiki/Radix_tree)
- [Patricia tree](https://xlinux.nist.gov/dads//HTML/patriciatree.html)
- [radix-tree.c](https://github.com/torvalds/linux/blob/master/lib/radix-tree.c)
- [PAT Tree and PAT Array](http://kontext.fraunhofer.de/haenelt/kurs/Referate/Koerkel-Qu-PATTrees.pdf)
- [PAT Tree 子串匹配结构](http://hxraid.iteye.com/blog/615295)
