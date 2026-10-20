# platform_365days 数据集

数据集由 6 个 ZIP 压缩包组成，使用 Git LFS 存储。

## 下载

请先安装 Git 和 [Git LFS](https://git-lfs.com/)，然后执行：

```bash
git lfs install
git clone https://github.com/ccecilia11/SHECTO_TEST.git
```

如果已经克隆仓库，但只得到很小的指针文件，请在仓库目录中执行：

```bash
git lfs pull
```

## 解压

下载全部 `platform_365days-part-001.zip` 至 `platform_365days-part-006.zip`。
这 6 个文件是可分别解压的 ZIP 包。请将所有压缩包解压到同一目录，合并其中的 `platform_365days` 文件夹。

Windows PowerShell 示例（在仓库目录中运行）：

```powershell
Get-ChildItem -Filter 'platform_365days-part-*.zip' | ForEach-Object {
    Expand-Archive -LiteralPath $_.FullName -DestinationPath './extracted'
}
```

解压后，数据位于 `extracted/platform_365days/`。
