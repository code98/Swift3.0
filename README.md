# Swift3.0
Swift 3.0 Preview 1更新内容中文翻译 http://www.liangkun.info</br>

##前言</br>
随着WWDC 2016的召开，苹果正式发布了Swift 3.0 Preview 1，这是苹果Swift3语言的首个稳定开发者预览版。苹果在其Swift.org官方博客中称，Preview 1版本比代码库中打包的Snapshot版本稳定很多。</br>

今天我翻译一下Swift 3.0 Preview</br>
1版本更新内容，能力有限翻译不到位的地方敬请谅解，如果有能力的同学可以自己查看官方英文版本。</br>
地址：https://swift.org/blog/swift-3-0-preview-1-released/</br>

##更新内容</br>
###中文版本：</br>
·       SE-0002: 删除currying的func声明语法</br>
·       SE-0003: 函数参数中不再使用var关键字</br>
·       SE-0004: 移除自增运算符++和自减运算符—-</br>
·       SE-0005: 将Objective-C的API更好地接入到Swift中</br>
·       SE-0006: 将API指南应用于标准库中</br>
·       SE-0007: 移除C语言风格的for循环（条件与增量下）</br>
·       SE-0008: 为可选序列增加一个Lazy的flatMap</br>
·       SE-0016: 添加构造函数Int和UInt进行UnsafePointer和UnsafeMutablePointer之间的转换</br>
·       SE-0017: 使用UnsafePointer时，修改Unmanaged</br>
·       SE-0019: Swift增加Testing</br>
·       SE-0023: Swift API设计指南</br>
·       SE-0028: 更新Swift的debug标识符（例如：__FILE__等）</br>
·       SE-0029: 从函数应用中，移除“tuple splat”表达形式</br>
·       SE-0031: 调整inout声明的类型修饰</br>
·       SE-0032: SequenceType添加first(where:)方法</br>
·       SE-0033: 导入Objective-C的常量作为Swift类型</br>
·       SE-0034: 消除行控制的Debug标识符声明的歧义</br>
·       SE-0037: 注释和操作符之间的交互</br>
·       SE-0039: 使Playground字面量现代化（Modernizing Playground Literals）</br>
·       SE-0040: 用冒号属性参数替换等号</br>
·       SE-0043: 声明变量时可以使用case标识符</br>
·       SE-0044: 导入成员</br>
·       SE-0046: 函数的所有参数声明方式要一致性，包括第一个参数声明方式</br>
·       SE-0047: 默认在非Void函数返回类型下，返回结果未使用时会有警告</br>
·       SE-0048: 泛型类型别名</br>
·       SE-0049: 将声明式@noescape与@autoclosure改为类型属性</br>
·       SE-0053: 从函数参数中移除let</br>
·       SE-0054: 废弃ImplicitlyUnwrappedOptional类型</br>
·       SE-0055: 明确不安全的Nullability指针使用Optional</br>
·       SE-0057: 导入Ovjective-C的轻量级泛型</br>
·       SE-0059: 更新API命名原则和重写的Set API</br>
·       SE-0061: 为autoreleasepool()添加通用结果和错误处理</br>
·       SE-0062: 引用Objective-C的关键路径</br>
·       SE-0064: 引用Objective-C的getters和setters的属性选择器</br>
·       SE-0065: 一种新的模型 Collections和Indices</br>
·       SE-0066: 规范函数类型必须使用括号</br>
·       SE-0069: 可变性和基础值类型</br>
·       SE-0070: 只在Objective-C下制定的Optional要求</br>
·       SE-0071: 允许成员引用使用most关键字</br>
·       SE-0085: 软件包管理器命令名称</br>
·       SE-0094: 为stdlib标准库添加sequence(first:next:) 和sequence(state:next:)</br>
</br>
</br>
###英文版本：</br>
·       SE-0002: Removing currying func declaration syntax</br>
·       SE-0003: Removing var from Function Parameters</br>
·       SE-0004: Remove the ++ and -- operators</br>
·       SE-0005: Better Translation of Objective-C APIs Into Swift</br>
·       SE-0006: Apply API Guidelines to the Standard Library</br>
·       SE-0007: Remove C-style for-loops with conditions and incrementers</br>
·       SE-0008: Add a Lazy flatMap for Sequences of Optionals</br>
·       SE-0016: Adding initializers to Int and UInt to convert from UnsafePointer and UnsafeMutablePointer</br>
·       SE-0017: Change Unmanaged to use UnsafePointer</br>
·       SE-0019: Swift Testing</br>
·       SE-0023: API Design Guidelines</br>
·       SE-0028: Modernizing Swift’s Debugging Identifiers (__FILE__, etc)</br>
·       SE-0029: Remove implicit tuple splat behavior from function applications</br>
·       SE-0031: Adjusting inout Declarations for Type Decoration</br>
·       SE-0032: Add first(where:) method to SequenceType</br>
·       SE-0033: Import Objective-C Constants as Swift Types</br>
·       SE-0034: Disambiguating Line Control Statements from Debugging Identifiers</br>
·       SE-0037: Clarify interaction between comments & operators</br>
·       SE-0039: Modernizing Playground Literals</br>
·       SE-0040: Replacing Equal Signs with Colons For Attribute Arguments</br>
·       SE-0043: Declare variables in ‘case’ labels with multiple patterns</br>
·       SE-0044: Import as Member</br>
·       SE-0046: Establish consistent label behavior across all parameters including first labels</br>
·       SE-0047: Defaulting non-Void functions so they warn on unused results</br>
·       SE-0048: Generic Type Aliases</br>
·       SE-0049: Move @noescape and @autoclosure to be type attributes</br>
·       SE-0053: Remove explicit use of let from Function Parameters</br>
·       SE-0054: Abolish ImplicitlyUnwrappedOptional type</br>
·       SE-0055: Make unsafe pointer nullability explicit using Optional</br>
·       SE-0057: Importing Objective-C Lightweight Generics</br>
·       SE-0059: Update API Naming Guidelines and Rewrite Set APIs Accordingly</br>
·       SE-0061: Add Generic Result and Error Handling to autoreleasepool()</br>
·       SE-0062: Referencing Objective-C key-paths</br>
·       SE-0064: Referencing the Objective-C selector of property getters and setters</br>
·       SE-0065: A New Model For Collections and Indices</br>
·       SE-0066: Standardize function type argument syntax to require parentheses</br>
·       SE-0069: Mutability and Foundation Value Types</br>
·       SE-0070: Make Optional Requirements Objective-C-only</br>
·       SE-0071: Allow (most) keywords in member references</br>
·       SE-0085: Package Manager Command Names</br>
·       SE-0094: Add sequence(first:next:) and sequence(state:next:) to the stdlib</br>
 
 
##下载</br>
Apple (Xcode)</br>
Swift 3.0 已经集成在Xcode8 beta 1里面。</br>
下载地址：https://developer.apple.com/xcode/download</br>

Linux (Ubuntu 14.04 and Ubuntu 15.10)</br>
为Ubuntu14.04和Ubuntu15.10提供的二进制文件下载地址：</br>
https://swift.org/download/</br>

##文档</br>
Swift 3.0的《The Swift
Programming Language》现在已经可以阅读了，地址：https://swift.org/documentation/#the-swift-programming-language</br>

你也可以在Apple的 iBooks</br>
Store里面阅读，地址：</br>
https://itunes.apple.com/us/book/the-swift-programming-language/id1002622538?mt=11</br>


##迁移到Swift 3</br>
Swift 3与Swift 2.2.1在代码上变化极大，包含了许多语法优化与更新，但在Objective-C</br>
API接入Swift的方式上也有巨大的变化（ SE-0005 ），请参见 迁移指南来查看迁移到Swift 3的指南与技巧。</br>
