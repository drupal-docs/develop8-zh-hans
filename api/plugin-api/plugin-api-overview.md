# Plugin API 概述

[原文地址](https://www.drupal.org/docs/8/api/plugin-api/plugin-api-overview)

`插件`是一种可插拔的小功能。执行类似功能的插件称为同一`插件类型`，也就是`plugin type`。

Drupal包含了很多不同类型的插件。比如，`Field widget` 是一个插件类型，
而每一个`Field widget plugin`是一个具体的插件。
管理员用户可以从`Field widget`插件列表中选择一个插件，设置为某一个字段所使用。

Drupal8 的插件系统提供了一系列的策略和可重用的代码组件，
让开发者方便地开发插件。

插件是在模块中定义的：一个模块可以提供不同插件类型的插件，
不同的模块可以提供自定义插件类型`plugin type`。

## 概述
- Plugin Types 插件类型

  `plugin type` 定义这一类型的插件，如何被系统发现以及如何实例化。
  还描述了此类型的插件所要做的事件。例如，缓存任务，图片处理，区块等等。
  
- Plugin Discovery 插件发现

  `插件发现`是系统在现有代码库中查找某一类型的所有可用插件的过程。

- Plugin Factory 插件工厂

  `插件工厂` 是用于实例化指定插件的。
  
另外，插件系统还提供了几个有用的组件，用于特定用途。

- Plugin Derivatives 插件指令
- Discovery Decorators 发现修饰器
- Plugin Mappers 插件映射

