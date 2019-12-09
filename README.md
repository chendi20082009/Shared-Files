# Shared-Files
https://help.github.com/cn/github/managing-large-files/what-is-my-disk-quota

我的磁盘配额是多少？
GitHub 没有任何设置的用户磁盘配额。 我们尝试为所有 Git 仓库提供丰富的存储空间，尽管文件和仓库大小存在硬性限制。 保持较小的仓库可确保我们的服务器速度较快，并且我们的用户可以快速下载。

Tip: If you regularly push large files to GitHub, consider introducing Git Large File Storage (Git LFS) as part of your workflow. Git LFS works well with the GitHub Flow and can be used with any large file, regardless of its type. For more information, see "Versioning large files."

文件和仓库大小限制
我们建议每个仓库均保持在 1GB 以下。 仓库的硬限制为 100GB。 如果达到 75GB，推送时您将在终端收到 Git 的警告。 如果将大文件留在仓库之外，则此限制很容易保持。 如果仓库超过 1GB，您可能会收到来自 GitHub 支持的礼貌电子邮件，要求您减小仓库的大小以使其恢复。

此外，我们严格限制大小超过 100 MB 的文件。 更多信息请参阅“使用大文件”。

注：如果您通过浏览器将文件添加到仓库，该文件不得大于 25 MB。 更多信息请参阅“添加文件到仓库”。

备份
Git 没有充分设计为用作备份工具。 However, there are many solutions specifically designed for performing backups that are worth checking out, including Arq, Carbonite, and CrashPlan.

数据库转储
大型 SQL 文件与 Git 等版本控制系统不兼容。 如果您希望为开发者提供最新的生产数据集，我们建议您使用 Dropbox 在开发者之间共享类似的文件。

如果您希望备份生产服务器，请参阅上面的备份部分。

外部依赖项
导致 Git 仓库变得庞大和膨胀的另一个原因是外部依赖项。 最好将这些文件留在仓库之外，并使用包管理器代替。 大多数流行的语言都附带包管理器，可以为您执行此操作。 Bundler、节点的包管理器和 Maven。 它们均支持直接使用 Git 仓库，因此您不需要预先打包的源。

打包的发行版本
我们不建议分发仓库中已编译的代码和预先打包的发行版。 有关共享大文件的更多信息，请参阅“分发大型二进制文件”。

更改现有仓库的历史记录
如果您已有一个相当大的仓库，不要担心！ 您可以从仓库的历史记录中删除大文件以缩减其大小。 更多信息请参阅“从仓库的历史记录中删除文件”。
