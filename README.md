# AdPsyche
This is a repository for AdPsyche, Japanese preference dataset based on advertising psychology.

## 📁 Dataset Files

This repository contains two main datasets used in our study on human preferences in advertisement. The datasets are intended for analyzing the relationship between user personality traits and ad appeal.

---

### `human_preference.csv`

This file contains pairwise comparison annotations of Japanese advertisements. Each row represents a human judgment about which of two ads is more appealing for the same product.

**Columns:**

| Column Name        | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `product_id`       | Unique identifier for the product                                           |
| `lp_text`          | Landing page text (contextual product description shown to annotators)     |
| `ad_text_a`        | First ad text (option A)                                        |
| `ad_text_b`        | Second ad text (option B)                                       |
| `appeal_type_a`    | Type of appeal for ad A (e.g., "無料"=free, "高品質"=High quality, etc.)         |
| `appeal_type_b`    | Type of appeal for ad B                                                     |
| `preferred_${user_id}` | Individual judgments from up to 109 annotators for each ad pair (e.g., `a. ad_text_a`, `b. ad_text_b`, or `same`) |




---

### `big5_zscores.csv`

This file contains standardized Big Five personality trait scores (z-scores) for each annotator in the dataset. It enables trait-based filtering and analysis across the participant group.

**Columns:**

| Column Name           | Description                                                           |
|-----------------------|-----------------------------------------------------------------------|
| `user_id`             | Unique identifier for the annotator (matches IDs used `human_preference.csv`)     |
| `gender`              | Annotator's gender (e.g., "男性" = male, "女性" = female)             |
| `age`                 | Age group (e.g., "30代" = 30s, "40代" = 40s, etc.)                     |
| `z_neuroticism`       | Z-score for Neuroticism                                               |
| `z_extraversion`      | Z-score for Extraversion                                              |
| `z_openness`          | Z-score for Openness                                                  |
| `z_agreeableness`     | Z-score for Agreeableness                                             |
| `z_conscientiousness` | Z-score for Conscientiousness  





---




# Citation
Thank you for your interest in our dataset. If you use it in your research, please cite:

```
@inproceedings{mita-etal-2025-adpsyche,
    title = "AdPsyche: 広告心理学に基づく選好データセット",
    author = "三田, 雅人  and
      村上, 聡一朗  and
      本多, 右京  and
      岡, 達志",
    booktitle = "言語処理学会 第31回年次大会 発表論文集",
    month = 3月,
    year = "2025",
    publisher = "言語処理学会",
    url = "https://www.anlp.jp/proceedings/annual_meeting/2025/pdf_dir/P10-13.pdf",
    pages = "4115--4120",
}
```

# License
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.](https://creativecommons.org/licenses/by-nc-sa/4.0/)
