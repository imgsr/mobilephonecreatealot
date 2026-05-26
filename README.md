# Phone Number to vCard Generator

一个简单的 Bash 脚本，用于从单个手机号生成 10,000 个连续号码的 vCard 联系人文件（.vcf），方便批量导入手机通讯录。

## 功能特点

- 输入一个 11 位手机号作为起始号码
- 自动生成 10,000 个连续号码（每次 +10000）
- 输出标准的 vCard 2.1 格式文件
- 支持自定义输出文件名
- 文件覆盖前会提示确认
- 支持 UTF-8 和 Quoted-Printable 编码

## 使用方法

1. 给脚本添加执行权限：
   ```bash
   chmod +x 电话号码生成脚本.sh
2. 按提示输入：
   · 11 位起始手机号
   · 输出文件名（可选，默认 contacts_generated.vcf）
3. 生成的 .vcf 文件可直接导入手机通讯录。

示例

```bash
请输入11位电话号码: 13800000000
请输入输出文件名（默认: contacts_generated.vcf）: my_contacts.vcf

正在生成联系人...
✅ 成功生成 10000 个联系人
📁 保存位置: /home/user/my_contacts.vcf
📞 号码范围: 从 13800000000 到 13899990000
```

注意事项

· 号码变化规律：每次在原号码上增加 10000
· 脚本会清空已存在的输出文件（覆盖前有确认提示）
· 生成的 vCard 中，联系人姓名与电话号码相同

许可证

MIT License

贡献

欢迎提交 Issue 或 Pull Request。

```
