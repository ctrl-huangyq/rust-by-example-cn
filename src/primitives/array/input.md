数组是一组包含相同数据类型 `T` 的组合，并存储在连续的内存区中。数组使用中括号 `[]` 来创建，
另外它们的大小在编译期间就已确定，数组的类型标记为 `[T; size]`（译注：T 为元素的类型，size
表示数组的大小）。

slice（中文有“切片”之意） 类型和数组类似，但 slice 类型的大小在编译期间是不确定的。相反，
slice 是一个双字对象（two-word object），第一个字是一个指向数据的指针，第二个字是切片的
长度。slice 可以用来借用数组的一部分。slice 的类型标记为 `&[T]`。

{array.play}