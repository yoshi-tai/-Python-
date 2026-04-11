# vscode-

このリポジトリには、Windows上のJava／Webアプリ開発用プロジェクトが含まれています。

## 含まれる主な項目
- `WebContent/`：Webアプリの公開フォルダ
- `src/main/java/`：Javaソース
- `APIDev00/`, `BatchDev00/`：Spring Bootプロジェクト
- `pom.xml`：ルートプロジェクトのMaven設定

## 実行方法例
### 1. ルートプロジェクトのビルド
```powershell
cd C:\vscode作成
mvn -e -DskipTests package
```

### 2. 各Spring Bootプロジェクトの実行
```powershell
cd C:\vscode作成\APIDev00
mvn spring-boot:run
```

```powershell
cd C:\vscode作成\BatchDev00\KKS06BJ01
java -jar target/demo-0.0.1-SNAPSHOT.jar
```

## 注意
- `target/` と `build/` はGit管理対象外にしています。
- EclipseやVS Codeでプロジェクトを開く際は、Maven設定を読み込んでください。

## リモート統合
このREADMEはリモートの既存内容とマージされています。