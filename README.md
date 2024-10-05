# Realtime-APIを使用したSotaとの会話

## 準備

1. 仮想環境を作成・立ち上げ
    - Mac / Linux

    ```zsh
    python -m venv .venv
    source .venv/bin/activate
    ```

    - Windows
  
    ``` powershell
    python -m venv .venv
    .venv\Scripts\activate
    ```

2. 必要パッケージのインストール

    ```zsh
    pip install -r requirements.txt
    ```

3. `.env`ファイルの作成
   `main.py`と同じ階層下に`.env`ファイルを作成し、以下を入力

    ```zsh
    OPENAI_API_KEY="APIKEY"
    ROBOT_IP="IP"
    ROBOT_PORT=PORT
    ```

4. 実行(ロボットがない場合は`mic.py`でパソコンで完結できます)

    ```zsh
    python robot.py
    ```

## 実装内容

SotaとRealtime-APIを使っておしゃべりができるコードを書きました。
少し聞き間違いもありますが基本的なことであれば問題なく話せます。
（参照：<https://zenn.dev/asap/articles/4368fd306b592a）>

> [!WARNING]
> robotの方はスピーカの音が大きいとマイクが拾ってしまいます。気をつけてしてください。
