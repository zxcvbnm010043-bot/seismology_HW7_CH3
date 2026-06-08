# 地震學 第三章：地震波與地球結構 (Seismology Chapter 3)

本目錄包含地震學課程第三章的講義教材以及一個用於繪製地震記錄剖面圖 (Record Section) 的 Python 腳本。

## 目錄內容

### 講義教材 (PDFs)
本章節涵蓋了從折射與反射地震學到地球內部結構的組成等主題：

- **3.1 Introduction**: 地震學導論 (15_3.1 Introduction.pdf)
- **3.2 Refraction seismology**: 折射地震學 (16_3.2 Refraction seismology.pdf)
- **3.3 Reflection seismology**: 反射地震學 (17_3.3 Reflection seismology.pdf)
- **3.4 Seismic waves in a spherical earth**: 球狀地球中的地震波 (18_3.4 Seismic waves in a spherical earth.pdf)
- **3.5 Body wave travel time studies**: 體波走時研究 (19_3.5 Body wave travel time studies.pdf)
- **3.6 Anisotropic earth structure**: 各向異性地球結構 (20_3.6 Anisotropic earth structure.pdf)
- **3.7 Attenuation and anelasticity**: 衰減與非彈性 (21_3.7 Attenuation and anelasticity.pdf)
- **3.8 Composition of the mantle and the core**: 地函與地核的組成 (22_3.8 Composition of the mantle and the core.pdf)

### 程式腳本
- **`seismicwave_sort.py`**: 
  - **功能**: 這是一個完整的、可執行的 Python 腳本，用於繪製地震波走時與波形剖面 (Record Section)。
  - **特點**: 
    - 包含模擬資料產生區塊，可直接執行展示。
    - 使用 `ObsPy` 處理地震資料，並使用 `Matplotlib` 繪圖。
    - 展示了如何將不同測站的波形根據距離 (Distance) 進行排列。

## 執行環境需求

若要執行 `seismicwave_sort.py`，請確保已安裝以下 Python 函式庫：

```bash
pip install pandas matplotlib numpy obspy
```

> **注意：** 目前已於 Conda 環境 `py3.9_1` 建立好包含 `obspy` 等套件的執行環境。
> - **環境名稱：** `py3.9_1`
> - **環境路徑：** `C:\Users\utaipei\miniconda3\envs\py3.9_1`

## 使用說明

1. **閱讀講義**: 建議按照編號順序 (3.1 到 3.8) 閱讀 PDF 檔案以建立完整的理論基礎。
2. **運行腳本**: 執行 `python seismicwave_sort.py` 即可查看模擬的地震波記錄剖面圖。
3. **自定義資料**: 若有真實地震資料，可參考 `seismicwave_sort.py` 中的註解，將模擬資料區塊替換為真實的讀取與處理流程。
