backend:
  name: github
  repo: ユーザー名/リポジトリ名
  branch: main

media_folder: "images"
public_folder: "/images"

collections:
  - name: "waittime"
    label: "待ち時間"
    files:
      - file: "data/wait.json"
        label: "待ち時間"
        name: "wait"
        fields:
          - { label: "待ち時間", name: "time", widget: "number" }
