<!--
Copyright 2023 Google LLC

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->
# sample-gas-on-aside

asideを使ってローカルでGASを開発してみる

## セットアップ手順

### TypeScriptとESLintのバージョン互換性問題の解決

プロジェクトで使用しているTypeScriptのバージョンが`@typescript-eslint`と互換性がない場合、以下の手順で解決できます。

1. 現在の`@typescript-eslint`パッケージをアンインストールします。
    ```bash
    npm uninstall @typescript-eslint/eslint-plugin @typescript-eslint/parser
    ```

2. サポートされているバージョンの`@typescript-eslint`パッケージをインストールします。
    ```bash
    npm install @typescript-eslint/eslint-plugin@5.59.0 @typescript-eslint/parser@5.59.0
    ```

3. サポートされているバージョンのTypeScriptをインストールします。
    ```bash
    npm install typescript@5.1.6
    ```
