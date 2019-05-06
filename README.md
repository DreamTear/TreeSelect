# TreeSelect
这是一个基于element UI 2.6 的下拉属，支持单选和多选，

# 使用方法
将src目录下的vue文件copy到自己的工程目录下，然后引入到需要的地方就可以使用了
# 特性
* 支持直接数据和远程加载数据
* 支持单选和多选
* 支持使用checkbox和不显示checkbox

# props
## multiple
类型: Boolean

默认值： false

设置下拉树是单选树还是多选数

## showValue
类型： [String, Array]

主要用于在下拉树未加载到已选中数据时，显示的数据名

## value
类型： [String, Array]

提交的值

## placeholder
类型： String

没有值是显示的占位内容

## disabled
类型： Boolean

设置下拉树不可用

## treeOption
类型： Object

使用树的配置项，和element ui中tree的选项几乎一致

主要配置项：
```
{
	data: null,
	lazy: false,
	load: null,
	props: {
		children: '',
		label: '',
		disabled: '',
		isLeaf: ''
	},
	key: '',// 配置树上使用的key
	showCheckbox: false,
	checkStrictly: false
}
