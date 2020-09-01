## 一、知识点

1. 为什么需要自动化对象映射？

因为项目开发经常遇到的两大核心问题：如何提高效率、如何提升质量。

2. 它可以做什么？

通过快速实现类对象间的映射（主要解决DTO与模型间的赋值转换）问题，减少编码，从而提高开发效率。

3. 主流技术方案
![Image text](show.png)


4. 性能对比

 	AutoMapper	TinyMapper
组件版本	9.0.0	3.0.2-beta
组件大小	268KB	53KB
最后更新时间	2019.08.12	2018.06.07
使用方式	静态方法、依赖注入	静态方法
自定义映射	支持、功能强大、灵活	支持
列表对象映射	支持	支持，需额外映射
性能（ms）	Add	32.75	2.34
Edit	19.93	1.63
Get	10.62	1.13
Pager(100)	103.54	146.22
Pager(5000)	233.18	147.94
三、总结

1. 通过上面的示例可以看到，使用自动化对象映射工具，比手工映射的代码量要少非常多，对系统开发而言，减少的工作量是非常可观的，可以大大加快开发效率。

2. 性能上，手工映射 > TinyMapper > AutoMapper，所以在局部复杂的映射上可以采用手工映射。



## Project Description
Powerful customisable tool for mapping entities to each other. Entities can be plain objects, DataReaders, SQL commands and anything you need. The tool uses run-time code generation via the Emit library. It is usefull for dealing with DTO objects, data access layers an so on.
## Supported platforms:

* Microsoft .NET Framework 3.5
* Microsoft Silverlight 3
* Mono
## About Emit Mapper

* Overview
* Benefits of Emit Mapper
* Getting started
* Type conversion
* Customization

# Customization overview

Customization using default configurator
* Default configurator overview
* Custom converters
* Custom converters_for_generics
* Null substitution
* Ignoring members
* Custom constructors
* Shallow and_deep_mapping
* Names matching
* Post processing

Low-level customization using custom configuratorors
# Emit Mapper in practice.

* Benchmark: EmitMapper vs Handwritten code vs AutoMapper
* Objects change tracking
* Mapping DbDatareader to objects
* Mapping objects to DbCommand (UPDATE and INSERT)
Last edited Jan 11, 2010 at 3:01 PM by romankovs, version 25
from http://emitmapper.codeplex.com/
