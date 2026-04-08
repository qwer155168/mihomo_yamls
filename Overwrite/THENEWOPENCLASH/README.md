# 📦 OpenClash 新版覆写模块

基于新版 OpenClash `[YAML]` 块覆写格式自动生成。

**设计原则：**
- 文件内所有覆写内容**默认全部注释**，加载后对你的现有配置零影响
- `proxy-providers` 原始内容完整复制进文件，对照修改 `url` 后取消注释即可替换订阅链接
- 提供完整操作符参考和逐类示例，按需取消注释即可实现规则追加、节点插入、批量更新等

**与旧版 `.conf` 的区别：**

| | 旧版 `.conf` | 新版 `.yaml` |
| :--- | :--- | :--- |
| url 替换 | `ruby_map_edit` + `$EN_KEY` 环境变量 | 直接写订阅链接，或用 `proxy-providers*` 条件更新 |
| 修改能力 | 仅能替换指定路径的值 | 合并/强制覆盖/追加/删除/批量条件更新 |
| 默认行为 | 启用后立即覆写 | 全部注释，零影响，按需解注释 |

## 📂 目录

| 分类 | 文件数 |
| :--- | :--- |
| 📁 **[General_Config/666OS](./General_Config/666OS/README.md)** | 2 个 |
| 📁 **[General_Config/ClashConnectRules](./General_Config/ClashConnectRules/README.md)** | 1 个 |
| 📁 **[General_Config/HenryChiao](./General_Config/HenryChiao/README.md)** | 3 个 |
| 📁 **[General_Config/Kerronex](./General_Config/Kerronex/README.md)** | 1 个 |
| 📁 **[General_Config/Lanlan13-14](./General_Config/Lanlan13-14/README.md)** | 3 个 |
| 📁 **[General_Config/Mitchell](./General_Config/Mitchell/README.md)** | 1 个 |
| 📁 **[General_Config/Repcz](./General_Config/Repcz/README.md)** | 2 个 |
| 📁 **[General_Config/SHICHUNHUI88](./General_Config/SHICHUNHUI88/README.md)** | 1 个 |
| 📁 **[General_Config/Seven1echo](./General_Config/Seven1echo/README.md)** | 2 个 |
| 📁 **[General_Config/echs-top](./General_Config/echs-top/README.md)** | 1 个 |
| 📁 **[General_Config/fufu](./General_Config/fufu/README.md)** | 1 个 |
| 📁 **[General_Config/iKeLee](./General_Config/iKeLee/README.md)** | 2 个 |
| 📁 **[General_Config/liandu2024](./General_Config/liandu2024/README.md)** | 5 个 |
| 📁 **[General_Config/liuran001](./General_Config/liuran001/README.md)** | 1 个 |
| 📁 **[General_Config/lvbibir](./General_Config/lvbibir/README.md)** | 1 个 |
| 📁 **[General_Config/qichiyuhub](./General_Config/qichiyuhub/README.md)** | 1 个 |
| 📁 **[General_Config/wanswu](./General_Config/wanswu/README.md)** | 1 个 |
| 📁 **[General_Config/yyhhyyyyyy](./General_Config/yyhhyyyyyy/README.md)** | 2 个 |
| 📁 **[Mobile_Modules/AkashaProxy](./Mobile_Modules/AkashaProxy/README.md)** | 1 个 |
| 📁 **[Mobile_Modules/BoxProxy](./Mobile_Modules/BoxProxy/README.md)** | 1 个 |
| 📁 **[Mobile_Modules/ClashMix](./Mobile_Modules/ClashMix/README.md)** | 1 个 |
| 📁 **[Mobile_Modules/Surfing](./Mobile_Modules/Surfing/README.md)** | 1 个 |
| 📁 **[Official_Examples/Metacubex](./Official_Examples/Metacubex/README.md)** | 2 个 |
| 📁 **[Smart_Mode/666OS](./Smart_Mode/666OS/README.md)** | 2 个 |
| 📁 **[Smart_Mode/HenryChiao](./Smart_Mode/HenryChiao/README.md)** | 4 个 |
| 📁 **[Smart_Mode/echs-top](./Smart_Mode/echs-top/README.md)** | 1 个 |
| 📁 **[Smart_Mode/edison](./Smart_Mode/edison/README.md)** | 1 个 |
| 📁 **[Smart_Mode/liandu2024](./Smart_Mode/liandu2024/README.md)** | 3 个 |
| 📁 **[Smart_Mode/qichiyuhub](./Smart_Mode/qichiyuhub/README.md)** | 1 个 |

## 🚀 使用方法

1. 找到对应分类目录，复制 `.yaml` 文件的 Raw URL
2. OpenClash → 覆写设置 → 覆写模块 → 添加该 URL
3. 打开文件，找到文件末尾的 `proxy-providers` 原始内容
4. 对照 `name:` 确认 provider 名称，参考文件内【订阅 URL 替换】示例写好替换内容
5. 取消注释对应内容保存，重启插件生效

[🏠 返回主页](../../README.md)