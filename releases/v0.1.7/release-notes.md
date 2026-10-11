# komopdf 0.1.7

## 文本编辑修复 / Text editing fixes

- 调整文本框大小不再缩放文字。拉宽、拉窄会按容器宽度换行；拉高只增加可见空间，保持字号、字形和字距。
- 框内暂时显示不全的内容完整保留；扩大高度后可显露，撤销、重做及保存重开后仍然有效。
- 原 PDF 字体与定位保留，新增中文和英文可正常编辑；连续调整框高不会反复改变原字形渲染。
- 提交文字修改时避免编辑层闪回旧内容。图片和矢量对象仍按原有方式缩放。

- Text handles now resize the layout frame instead of scaling PDF glyphs. Width changes wrap text; height changes reveal retained lines without changing font size or spacing.
- Clipped text is retained through undo/redo and saved PDF reopening. Repeated height changes preserve the original glyph operators.
- Original PDF fonts are retained. CJK and Latin additions, normal commit rendering, and image/path scaling are covered by regression checks.

## 下载 / Download

Windows x64，Windows 10 22H2 或更新版本。提供完整离线运行时与第三方许可。此版本没有新增 macOS 安装包。

非 AI PDF 功能继续免费、无需登录。账户、积分和订阅规则不变。

The shared web editor and PDF engine are open source. GitHub's automatic source archives contain this release repository's public documentation, not the private desktop source or an installer.
