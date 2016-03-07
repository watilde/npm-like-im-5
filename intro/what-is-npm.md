# npmとは何か？

npmとは、JavaScriptのためのパッケージマネジャーです。
2つの主要なゴールが存在します：

- コードを簡単に利用できる場所に配置する
- 異なるバージョンの依存しているパッケージを管理する

npmは、3つの主要なプロダクトを以て達成しようとしています：

- コマンド
- レジストリ
- ウェブサイト

## コマンド

npmのコマンドは、ターミナルでレジストリと会話を行うためのプログラムです。
これは、今のところ最も知られているnpmのプロダクトとなります。

## レジストリ

npmのレジストリは、npmが持っている最も貴重な資産です。レジストリとは、
全てのパッケージのデータと、そのメタデータを含む
データベース(実際は複数のデータベース！)のことを指します。

`npm install` (他のコマンドも！)を実行した際には、npmの
レジストリへのリクエストが生成されます。

実際は、npmコマンドは *どのような* レジストリとも使うことができます。
npmレジストリは、単にデフォルトの設定であるということです。

### npm OnSite

npm OnSite is a paid product by which npm provides customers
with a fully replicated version of the public registry for use
behind company firewalls.

## The Website

The website is npm's home on the World Wide Web. It has two primary goals:

- display package READMEs
- allow users to manage package permissions via Orgs and Teams

### Package READMEs

The primary function of the website is to allow users to search
for packages and read information on them. Information on each
package is found in a `README.md` file in the root directory of
the package repository (often, GitHub).

npm uses a package called [`marky-markdown`] to parse package `README`s
and displays it on the website. It attempts to parse and display the
files exactly as GitHub does, but currently is not.
there.

### Orgs and Teams

As of last November, npm offers a new service called ["Orgs and Teams"]
which grants users the ability to manage permissions to packages.

This is currently only a paid product, but an open source tier will be
available in the future.

[`marky-markdown`]: https://github.com/npm/marky-markdown
["Orgs and Teams"]: https://docs.npmjs.com/orgs/what-are-orgs
