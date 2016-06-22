# Swift3.0
Swift 3.0 Preview 1更新内容中文翻译 http://www.liangkun.info

前言
随着WWDC 2016的召开，苹果正式发布了Swift 3.0 Preview 1，这是苹果Swift 3语言的首个稳定开发者预览版。苹果在其Swift.org官方博客中称，Preview 1版本比代码库中打包的Snapshot版本稳定很多。

今天我翻译一下Swift 3.0 Preview
1版本更新内容，能力有限翻译不到位的地方敬请谅解，如果有能力的同学可以自己查看官方英文版本。
地址：https://swift.org/blog/swift-3-0-preview-1-released/

更新内容
中文版本：
·       SE-0002: 删除currying的func声明语法
·       SE-0003: 函数参数中不再使用var关键字
·       SE-0004: 移除自增运算符++和自减运算符—
·       SE-0005: 将Objective-C的API更好地接入到Swift中
·       SE-0006: 将API指南应用于标准库中
·       SE-0007: 移除C语言风格的for循环（条件与增量下）
·       SE-0008: 为可选序列增加一个Lazy的flatMap
·       SE-0016: 添加构造函数Int和UInt进行UnsafePointer和UnsafeMutablePointer之间的转换
·       SE-0017: 使用UnsafePointer时，修改Unmanaged
·       SE-0019: Swift增加Testing
·       SE-0023: Swift API设计指南
·       SE-0028: 更新Swift的debug标识符（例如：__FILE__等）
·       SE-0029: 从函数应用中，移除“tuple splat”表达形式
·       SE-0031: 调整inout声明的类型修饰
·       SE-0032: SequenceType添加first(where:)方法
·       SE-0033: 导入Objective-C的常量作为Swift类型
·       SE-0034: 消除行控制的Debug标识符声明的歧义
·       SE-0037: 注释和操作符之间的交互
·       SE-0039: 使Playground字面量现代化（Modernizing Playground Literals）
·       SE-0040: 用冒号属性参数替换等号
·       SE-0043: 声明变量时可以使用case标识符
·       SE-0044: 导入成员
·       SE-0046: 函数的所有参数声明方式要一致性，包括第一个参数声明方式
·       SE-0047: 默认在非Void函数返回类型下，返回结果未使用时会有警告
·       SE-0048: 泛型类型别名
·       SE-0049: 将声明式@noescape与@autoclosure改为类型属性
·       SE-0053: 从函数参数中移除let
·       SE-0054: 废弃ImplicitlyUnwrappedOptional类型
·       SE-0055: 明确不安全的Nullability指针使用Optional
·       SE-0057: 导入Ovjective-C的轻量级泛型
·       SE-0059: 更新API命名原则和重写的Set API
·       SE-0061: 为autoreleasepool()添加通用结果和错误处理
·       SE-0062: 引用Objective-C的关键路径
·       SE-0064: 引用Objective-C的getters和setters的属性选择器
·       SE-0065: 一种新的模型 Collections和Indices
·       SE-0066: 规范函数类型必须使用括号
·       SE-0069: 可变性和基础值类型
·       SE-0070: 只在Objective-C下制定的Optional要求
·       SE-0071: 允许成员引用使用most关键字
·       SE-0085: 软件包管理器命令名称
·       SE-0094: 为stdlib标准库添加sequence(first:next:) 和sequence(state:next:)


英文版本：
·       SE-0002: Removing currying func declaration syntax
·       SE-0003: Removing var from Function Parameters
·       SE-0004: Remove the ++ and -- operators
·       SE-0005: Better Translation of Objective-C APIs Into Swift
·       SE-0006: Apply API Guidelines to the Standard Library
·       SE-0007: Remove C-style for-loops with conditions and incrementers
·       SE-0008: Add a Lazy flatMap for Sequences of Optionals
·       SE-0016: Adding initializers to Int and UInt to convert from UnsafePointer and UnsafeMutablePointer
·       SE-0017: Change Unmanaged to use UnsafePointer
·       SE-0019: Swift Testing
·       SE-0023: API Design Guidelines
·       SE-0028: Modernizing Swift’s Debugging Identifiers (__FILE__, etc)
·       SE-0029: Remove implicit tuple splat behavior from function applications
·       SE-0031: Adjusting inout Declarations for Type Decoration
·       SE-0032: Add first(where:) method to SequenceType
·       SE-0033: Import Objective-C Constants as Swift Types
·       SE-0034: Disambiguating Line Control Statements from Debugging Identifiers
·       SE-0037: Clarify interaction between comments & operators
·       SE-0039: Modernizing Playground Literals
·       SE-0040: Replacing Equal Signs with Colons For Attribute Arguments
·       SE-0043: Declare variables in ‘case’ labels with multiple patterns
·       SE-0044: Import as Member
·       SE-0046: Establish consistent label behavior across all parameters including first labels
·       SE-0047: Defaulting non-Void functions so they warn on unused results
·       SE-0048: Generic Type Aliases
·       SE-0049: Move @noescape and @autoclosure to be type attributes
·       SE-0053: Remove explicit use of let from Function Parameters
·       SE-0054: Abolish ImplicitlyUnwrappedOptional type
·       SE-0055: Make unsafe pointer nullability explicit using Optional
·       SE-0057: Importing Objective-C Lightweight Generics
·       SE-0059: Update API Naming Guidelines and Rewrite Set APIs Accordingly
·       SE-0061: Add Generic Result and Error Handling to autoreleasepool()
·       SE-0062: Referencing Objective-C key-paths
·       SE-0064: Referencing the Objective-C selector of property getters and setters
·       SE-0065: A New Model For Collections and Indices
·       SE-0066: Standardize function type argument syntax to require parentheses
·       SE-0069: Mutability and Foundation Value Types
·       SE-0070: Make Optional Requirements Objective-C-only
·       SE-0071: Allow (most) keywords in member references
·       SE-0085: Package Manager Command Names
·       SE-0094: Add sequence(first:next:) and sequence(state:next:) to the stdlib
 
 
下载
Apple (Xcode)
Swift 3.0 已经集成在Xcode8 beta 1里面。
下载地址：https://developer.apple.com/xcode/download

Linux (Ubuntu 14.04 and Ubuntu 15.10)
为Ubuntu14.04和Ubuntu15.10提供的二进制文件下载地址：
https://swift.org/download/

文档
Swift 3.0的《The Swift
Programming Language》现在已经可以阅读了，地址：https://swift.org/documentation/#the-swift-programming-language

你也可以在Apple的 iBooks
Store里面阅读，地址：
https://itunes.apple.com/us/book/the-swift-programming-language/id1002622538?mt=11


迁移到Swift 3
Swift 3与Swift 2.2.1在代码上变化极大，包含了许多语法优化与更新，但在Objective-C
API接入Swift的方式上也有巨大的变化（ SE-0005 ），请参见 迁移指南来查看迁移到Swift 3的指南与技巧。
