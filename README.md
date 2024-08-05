物品管理系统
简介
这是一个使用 Python 和 tkinter 库构建的物品管理系统。用户可以通过图形用户界面添加、查找、查看统计信息、清空数据和备份数据。所有数据以 JSON 格式存储在一个本地文件中，确保数据的持久性和可操作性。

功能
添加物品：允许用户输入房间、收纳处和物品名称，并将其添加到数据文件中。
查找物品：根据物品名称查找其所在的房间和收纳处。
统计信息：显示当前记录的房间数量以及每个房间和收纳处中的物品数量。
清空数据：允许用户清空所有数据或选择特定房间或收纳处的数据。
备份数据：将当前的数据备份到用户指定的 JSON 文件中。
使用方法
运行程序
在命令行中执行以下命令来运行程序：

bash
Copy code
python <脚本文件名>.py
主要界面
程序启动后，会显示一个主窗口，包括一个按钮“打开主菜单”，点击该按钮可以进入主菜单。

主菜单功能
添加物品：打开一个新窗口，用户可以输入房间、收纳处和物品，然后提交以添加到数据文件。
查找物品：打开一个新窗口，用户可以输入物品名称进行查找，系统会显示物品的存放位置。
统计信息：显示系统中的房间和物品统计信息。
设置：提供清空数据和备份数据的选项。
清空数据
在设置窗口中，用户可以选择清空所有数据、特定房间的数据或特定收纳处的数据。执行清空操作后，相关数据将被删除。

备份数据
在设置窗口中，用户可以备份当前的数据到一个 JSON 文件中，确保数据不会丢失。

技术细节
数据存储：所有数据存储在名为 storage_data.json 的 JSON 文件中。该文件与脚本文件位于同一目录。
数据操作：使用 Python 内置的 json 库进行数据的读写操作。
用户界面：使用 tkinter 库构建 GUI，包括窗口、标签、输入框、按钮等。
注意事项
确保在执行程序时，脚本文件所在目录具有读写权限，以便正常创建和操作 JSON 数据文件。
由于数据是以 JSON 格式存储的，用户应避免直接修改 JSON 文件的内容，除非具备相应的技术能力。
许可
本项目遵循 MIT 许可 协议，详情请参阅 LICENSE 文件。