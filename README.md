# ぬいぐるみGPT

ぬいぐるみGPTはぬいぐるみを通して、ChatGPTと会話を行うシステムである

# Features
マイク入力をWhisper APIで文字起こしし、音声から起こした文字をChatGPT APIに投げて返答をVOICEVOXに渡すことによってChatGPTとの会話を行う
以下がシステムの概要図である
![スクリーンショット 2023-10-13 16 50 24](https://github.com/sophytoeat/TeddyGPT/assets/54713904/30a28d3c-6a5a-473c-b463-de35ad77c4b9)

# Installation
openai 0.27.0
``` pip install openai ```でインストロール

SpeechRecognition
``` pip install git+https://github.com/Uberi/speech_recognition ```でインストロール

PyAudio 0.2.13
``` pip install pyaudio ```でインストロール

VOICEVOX
https://voicevox.hiroshiba.jp/　からダウンロードしてください

# Usage
VOICEVOXを起動させた状態で```python main.py```で実行することが出来る
現状長めの文章だと返答に少し時間がかかります
```終わり```や```会話終了```といった会話を終了する内容で話しかけられた場合にシステムが終了します
