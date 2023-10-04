---
title: Hello HomeLab
dare: 2023-9-20 12:00:00 -500
categories:: [concept]
tags: [Introduction to Computer]
---

:::success
**計算機概論**

> [time=Sat, Aug 26, 2023 1:43 AM]
> :::
> operation 運行時間
> device 設備
> process 過程
> program 程式
> Kernel 核心
> Block 停，屏蔽
> Control 控制
> mode 模式
> state 狀態
> Context 上下文
> multitasking 多工
> Thread 執行序

堆疊與佇列 Stack and Queue
State Diagram 狀態圖
Long-term Scheduler 長期調度程序
Short-term Scheduler 短期適度程序

# Computer introduce

## Computer

- 特性
  - fast
  - big
  - accuracy(準確性)
- 硬體
  - CPU
  - 記憶體
  - 螢幕
- 軟體
  - 與硬體溝通
  - 與使用者溝通
- 韌體
  - **硬體中的軟體**
  - 被電腦執行的程式
- 作業系統
  - 管理硬體與軟體資源的程式
- 圖靈模型
  - 思路
    - 輸入
    - 程式處理
    - 輸出
- Von Neumann
  - 思路
    - 輸入
    - 控制單元(CU)，邏輯單元(ALU;arithmetic logic unit)，Memory
    - 輸出
  - 內儲程式(將程式存在記憶體)
- Von Neumann 瓶頸
  - CPU 在 I/O 記憶體時間閒置，因需在 CPU 跟記憶體之間匯流排交互
  - 增加匯流排可改善
- 程序指的是執行中的 program(程式)
- 1KB=10^3^=2^10^

---

## machine cycle

- 執行一個指令的週期(I-Time + E-Time)
- I-Time
  - 指令擷取
  - 解碼
  - 運算
- E-Time
  - 執行
  - 儲存

---

## CPU

- CPU 組成
  - CU+ALU
    - ALU=AU(算術單元 arithmetic unit)+LU(邏輯單元 Logic Unit)
- CPU 種類
  - RISC(精簡指令 Reduced Instruction Set Computer)
    - CPI 較短
    - 5 種定址模式
  - CISC(複雜指令 Complex Instruction Set Computer)
    - 10~20 種定址模式
- 效能標準
  - CPI(指令平均週期數 clock cycle per instruction)
  - MIPS
  - MTLOPS

---

# digital system and data storage

- 資料呈現方式
  - 類比:連續
  - 數位:間斷
  - 多媒體:兩種以上的資訊
- 資料儲存方法
  - 轉成數位
  - 英文需 1 位元，中文需 2 位元
- 數位碼類型
  - 二進碼十進數 Binary-Coded Decimal
  - Excuss-3 超三碼
  - Gray code 格雷碼
    - 因在轉換時二進位需換兩格(例:3 011,4 100)
    - 我理解為與二進位相對，從大的開始表示
- 文字表示法
  - ASCII
  - BIG5 繁體中文
  - Unicode 萬國碼
- 三原色(紅綠藍)
  - 一種顏色用 8bit
  - 一個全彩用三個顏色表示(24bit)
- 聲音
  - 取樣
    - 類比訊號是取點
  - 量化
    - 只要整數，小數四捨五入
  - R(位元率)=S(每秒樣本數)\*B(每個樣本位元數)
- 二補數
  - 表示正數跟負數
    - 正數 = 正數的 n-1 補數 + 1
    - 二補數 = 一補數 + 1
    - 用於運算
    - 減法就是先把負數用二補數變成正數表示法再做相加
- 浮點數表示法
  - 正負(0 或 1) + 位移量 + 定點數
  - 符號 + 指數 + 尾數
    - 符號 0 為正，1 為負
    - 指數
      - 超碼表示法就是存指數的方法
      - 定義小數點移位
    - 尾數
      - 以定點數記法存尾數
      - 定義精準度
  - 精確
  - 定點表示法
    - 小數點在最右邊(20.)
    - 僅整數
  - 浮點表示法
    - 實數=整數+分數
    - 實數不該整數太大
    - 實數不該分數不該太小
  - 正規化
    - 小數點左邊是一個非 0 的數
    - 科學方法(十進位)
    - 浮點數方法(二進位)
- 超碼系統
  - 都存成無號整數
  - 超[裡面是偏移量]
- 編碼與壓縮 - 變動長度編碼 - 霍夫曼編碼 - 字典編碼
  漢明碼有錯誤更正能力
  unicode 用 16bit 表示一個字元
  取樣頻率 44.1KHz 最接近真實的聲音
  顯示器[]\*[]個像素(Pixel)來表示解析度

- 輸入單元(CU)
