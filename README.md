# Subversion入門 for Windows

高野 将

## はじめに

本文書はVCS（Version Control System：バージョン管理システム）の一つであるSubversion（SVN）の概念、使い方を、未経験者でもわかるように伝えることを目的としています。本文書のゴールは以下の通りです。

- SVNの概念を理解する。
- SVNで基本的な操作ができる。
- SVNで競合解決などチーム連携作業ができる。
- SVNでタグ、ブランチ、マージを活用できる。

なお、OSはWindows、SubversionクライアントにはTortoiseSVNを利用します。CUIでのsvnコマンドの詳細なオプション、使い方については本書の対象外とします。

また、「[VCS入門](https://github.com/masaru-b-cl/introduction-to-vcs)」を既に読み終えていることを前提としています。読んでいない方は、まずこちらからどうぞ。

## 目次

1. [Subversion（SVN）とは？](1.what-is-svn.md "Subversion（SVN）とは？")
1. [SVNの導入](2.installing-svn.md "SVNの導入")
1. [個人での利用 - リポジトリの作成からインポート](3.personal-use-1.md "個人での利用 - リポジトリの作成からインポート")
1. [個人での利用 - 作業コピーの作成から最初のコミット](4.personal-use-2.md "個人での利用 - 作業コピーの作成から最初のコミット")
1. [個人での利用 - 追加と削除](5.personal-use-3.md "個人での利用 - 追加と削除")
1. [個人での利用 - 変更を元に戻す](6.personal-use-4.md "個人での利用 - 変更を元に戻す")
1. [個人での利用 - 除外設定](7.personal-use-5.md "個人での利用 - 除外設定")
1. [タグとブランチ - デフォルトフォルダー構造](8.tag-and-branch-1.md "タグとブランチ - デフォルトフォルダー構造")
1. [タグとブランチ - タグの作成](9.tag-and-branch-2.md "タグとブランチ - タグの作成")
1. [タグとブランチ - タグの復元とエクスポート](10.tag-and-branch-3.md "タグとブランチ - タグの復元とエクスポート")
1. [タグとブランチ - ブランチの作成、チェックアウト](11.tag-and-branch-4.md "タグとブランチ - ブランチの作成、チェックアウト")
1. [タグとブランチ - ブランチの変更、マージ](12.tag-and-branch-5.md "タグとブランチ - ブランチの変更、マージ")
1. [チームでの利用 - 作業ベース](13.team-use-1.md "チームでの利用 - 作業ベース")
1. [チームでの利用 - 競合の解決](14.team-use-2.md "チームでの利用 - 競合の解決")
1. [チームでの利用 - より進んだ運用](15.team-use-3.md "チームでの利用 - より進んだ運用")

## ライセンス
<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.ja"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a>

この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.ja">クリエイティブ・コモンズ 表示 - 継承 3.0 非移植 ライセンスの下に提供されています。</a>