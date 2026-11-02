---
name: geoskill-sar-crop-classification
description: '基于多时相 SAR 后向散射时序的农作物分类：逐像元时序/统计/物候特征 + 随机森林。SAR crop classification from multi-temporal backscatter time series using per-pixel phenological features and Random Forest. 合成模式生成水稻/小麦/玉米三类时序真值并评估精度，输出分类 GeoTIFF + 面积统计 + 混淆矩阵 JSON。'
---

# SAR农作物分类 | SAR Crop Classification

(Fill in 2-3 paragraphs of Chinese introduction here: features, application scenarios, core algorithm.)

## Dependencies / 依赖

```bash
pip install 'numpy' 'rasterio' 'scipy' 'scikit-learn'
```

## Usage / 使用方法

### Basic Usage

```bash
python geoskill-sar-crop-classification.py --bbox 116.0 39.0 117.0 40.0 [other options]
```

### Example 1 (synthetic data, offline)

```bash
python geoskill-sar-crop-classification.py --bbox 116.0 39.0 117.0 40.0 --synthetic --output-dir ./out
```

### Examples 2-5

(Add at least 4 real usage examples.)

## Output / 输出

| File | Format | Description |
|---|---|---|
| `result.tif` | GeoTIFF | Primary output |
| `output-manifest.json` | JSON | Run manifest |

## Data Source / 数据源 / Source

(Describe the data source: free satellite data / local input / synthetic.)

## Privacy / 隐私声明 / Privacy

- Runs offline by default; `--synthetic` mode is fully network-free.
- All processing is done locally; no user data is uploaded.

## License / License

MIT

---

> 中文完整版：需要时再读 [references/SKILL.zh-CN.md](references/SKILL.zh-CN.md)，不要默认全量加载。
