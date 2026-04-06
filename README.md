# 作業六：空間預測對決 + 期末專案提案

## 專案概述

此作業範例選用2025年7月28日的0728豪雨事件，以及2025年11月11日的鳳凰颱風，分析範圍為宜蘭縣以及花蓮縣。兩者在該地的降雨型態上有所不同，前者對東部地區影響不大，且降雨範圍較為平均。而後者受外圍環流與東北季風的共伴效應，則對北部及東部地區帶來致災性的超大豪雨。

本專案以此進行1000m網格的降雨量推估與比較分析，探討不同雨量內插與演算法在空間特徵捕捉上的差異。

## 工作流程

包含以下階段：

1. 資料前處理 (Data Preprocessing)
2. 空間變異分析 (Variogram Modeling)
3. 四大內插方法比較 (Prediction Shootout)
4. 不確定性分析 (Uncertainty Analysis)
5. 成果匯出 (GeoTIFF Export)


## 檔案結構

- `Week6_Shootout.ipynb` - Jupyter Notebook，主程式
- `README.md` - 本檔案，提供專案概述與說明
- `data/` - 目錄，包含降雨資料：
  - `rain_20250728.csv` - 2025年7月28日降雨資料(0728豪雨事件)
  - `rain_20251111.csv` - 2025年11月11日降雨資料(鳳凰颱風事件)
- `output/` - 目錄，包含生成的分析結果：
  - `0728豪雨_1_四種內插比較圖.png` 
  - `0728豪雨_2_差異圖.png`
  - `0728豪雨_3_SigmaMap.png` 
  - `鳳凰颱風_1_四種內插比較圖.png` 
  - `鳳凰颱風_2_差異圖.png` 
  - `鳳凰颱風_3_SigmaMap.png` 
- `fungwong_kriging_rainfall.tif` - 鳳凰颱風kriging金降雨資料TIFF檔
- `fungwong_kriging_variance.tif` - 鳳凰颱風kriging變異數資料TIFF檔
- `fungwong_rf_rainfall.tif` - 鳳凰颱風RF降雨資料TIFF檔
- `遙測空間應用_期末專題初稿.pdf` - 期末專題初稿PDF檔案
