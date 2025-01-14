---
title: "备份存储"
weight: 5
description: >
    备份存储提供更加完整、安全、稳定的数据备份。
---

备份存储提供更加完整、安全、稳定的数据备份。


**入口**：在云管平台单击左上角![](../../images/intro/nav.png)导航菜单，在弹出的左侧菜单栏中单击 **_"存储/备份存储/备份存储"_** 菜单项，进入备份存储页面。

![](../../images/storage/backup.png)

## 新建备份存储

该功能用于新建备份存储。

1. 在备份存储页面，单击列表上方 **_"新建"_** 按钮，弹出新建备份存储对话框。
2. 设置以下参数：
   - 指定域：管理员和域管理员在新建备份存储时需要指定备份存储的所属域。
   - 名称：设置备份存储的名称。备份存储名称全局唯一，不建议使用常用名称如test等，以防创建失败。
   - 备注：设置备份存储的备注。
   - 存储类型：支持NFS。
   - NFS Host：必须输入指定NFS Host。
   - NFS Shared Dir：必须输入指定NFS Shared Dir。
3. 单击 **_"确定"_** 按钮，创建备份存储。

## 同步状态

该功能用于获取备份存储的当前状态。

**单个同步状态**

1. 在备份存储页面，单击备份存储右侧操作列 **_"同步状态"_** 按钮，同步备份存储状态。

**批量同步状态**

1. 在备份存储列表中勾选一个或多个备份存储，单击 **_"批量操作"_** 按钮，选择 **_"同步状态"_** 菜单项，批量同步备份存储状态。

## 设置共享

该功能用于设置备份存储的共享范围。

**单个备份存储设置共享**

1. 在备份存储页面，单击备份存储右侧操作列 **_"更多"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数。
   - 当共享范围选择为“不共享”时，即项目资源的共享范围为私有，仅本项目的用户可以使用。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即项目资源的共享范围为域共享-部分，只有项目资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即项目资源的共享范围为域共享-全部，系统中的所有用户都可以使用项目资源。
3. 单击 **_"确定"_** 按钮，完成操作。

**批量设置共享**

多个备份存储批量设置的共享范围必须相同。否则请单独为备份存储设置共享。

1. 在备份存储列表中选择一个或多个备份存储，单击列表上方 **_"批量操作"_** 按钮，选择下拉菜单 **_"设置共享"_** 菜单项，弹出设置共享对话框。
2. 配置以下参数。
   - 当共享范围选择为“不共享”时，即项目资源的共享范围为私有，仅本项目的用户可以使用。
   - 当共享范围选择为“域共享”时，需要选择共享的域。
       - 当域选择其中的一个或多个域时，即项目资源的共享范围为域共享-部分，只有项目资源所在域和共享域下的用户可以使用域资源。
       - 当域选择全部时，即项目资源的共享范围为域共享-全部，系统中的所有用户都可以使用项目资源。
3. 单击 **_"确定"_** 按钮，完成操作。

{{% alert title="说明" %}}
设置域共享的条件：

- 在{{<oem_name>}}平台已开启三级权限。
- 用户处于管理后台。

{{% /alert %}}

## 删除备份存储

该功能用于删除备份存储，当备份存储中不存在文件时，才可以删除。


**单个删除**

1. 在备份存储页面，单击备份存储右侧操作列 **_"更多"_** 按钮，选择 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

**批量删除**

1. 在备份存储列表中勾选一个或多个备份存储，单击 **_"批量操作"_** 按钮，选择 **_"删除"_** 菜单项，弹出操作确认对话框。
2. 单击 **_"确定"_** 按钮，完成操作。

## 查看备份存储详情

该功能用于查看备份存储的详细信息。

1. 在备份存储页面，单击备份存储名称项，进入备份存储详情页面。
2. 查看以下信息：
   - 基本信息：云上ID、ID、名称、状态、域、标签、共享范围、存储类型、NFS Host、NFS Shared Dir、创建时间、更新时间、备注。

## 查看操作日志

该功能用于查看备份存储相关操作的日志信息。

1. 在备份存储页面，单击备份存储的名称项，进入备份存储详情页面。
2. 单击“操作日志”页签，进入操作日志页面。
   - 加载更多日志：列表默认显示100条操作日志信息，如需查看更多操作日志，请单击 “加载更多” 按钮，获取更多日志信息。
   - 查看日志详情：单击操作日志右侧操作列 “查看” 按钮，查看日志的详情信息。支持复制详情内容。
   - 查看指定时间段的日志：如需查看某个时间段的操作日志，在列表上方的搜索框中选择操作时间-范围选择，设置好开始时间和结束时间，查询指定时间段的日志信息。
   - 导出日志：目前仅支持导出本页显示的日志。单击右上角图标，在弹出的导出数据对话框中，设置导出数据列，单击 “确定” 按钮，导出日志。