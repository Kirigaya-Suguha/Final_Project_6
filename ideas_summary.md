1. 政策严格指数与确诊/死亡数据对比---------多轴折线图
   X 轴：时间
   Y 轴 1：政策严格指数（或者政策 string）
   Y 轴 2：每日新增确诊病例数（new_cases）或新增死亡数（new_deaths）
   分析思路：
   展示政策收紧或放松对新增病例和死亡人数的影响。
   比较不同国家政策实施时间与疫情控制效果的差异

2. 累计病例/死亡与疫苗接种的关系----------散点图
   X 轴：累计接种疫苗剂次占比（people_vaccinated_per_hundred）
   Y 轴：累计确诊病例（total_cases）或累计死亡人数（total_deaths）
   分组：国家
   分析思路：
   探讨疫苗接种覆盖率与疫情严重程度的关系。比较疫苗接种速度对疫情减缓的影响。

3. 经济发展与疫情严重程度-----散点图
   X 轴：gdp_per_capita
   Y 轴：total_cases_per_million 或 total_deaths_per_million
   分析思路：
   观察经济发达国家是否更容易减少死亡率或确诊率。

4. 医疗资源与死亡率的关系-----散点图
   图表类型：散点图或气泡图（每千人医院床位数）
   X 轴：hospital_beds_per_thousand
   Y 轴：total_deaths_per_million
   分析思路：
   观察医疗资源是否影响疫情中死亡人数的多少。

5. 健康水平与疫情传播的关系----散点图或线性回归图
   问题：健康水平较高的国家是否更能控制疫情？
   分析方法：
   X 轴：life_expectancy（人均预期寿命）
   Y 轴：total_cases_per_million 或 reproduction_rate（疫情传播速度）
   分析思路：
   长寿通常与良好的医疗系统和健康水平相关，可能影响疫情传播速度和确诊率。
   验证是否健康水平较高的国家，疫情更容易被控制。

## Chen Huaxun

1. 新增病例数 vs. 学校关闭政策

   疫情指标: new_cases_per_million（每百万人新增病例数）
   政策: C1M_School closing（学校关闭政策，0 到 3 级严格程度）
   分析目标:
   探讨不同国家实施学校关闭政策前后，每百万人新增病例数的趋势。
   假设: 严格关闭学校可能减少病毒传播，尤其在年轻人接触密集的情况下。

2. 新增死亡数 vs. 口罩政策

   疫情指标: new_deaths_per_million（每百万人新增死亡数）
   政策: H6M_Facial Coverings（口罩政策，0 到 4 级严格程度）
   分析目标:
   比较口罩政策实施前后，不同国家的死亡人数趋势。
   假设: 强制口罩政策减少病毒空气传播，从而间接降低重症率和死亡率。

3. 基本传染数 vs. 接触者追踪

   疫情指标: reproduction_rate（基本传染数，R 值）
   政策: H3_Contact tracing（接触者追踪，0 到 3 级严格程度）
   分析目标:
   探讨追踪接触者的政策是否有效降低基本传染数。
   假设: 接触追踪提高了潜在感染者的隔离效率，从而减少病毒传播。

4. 阳性率 vs. 检测政策

   疫情指标: positive_rate（检测阳性率）
   政策: H2_Testing policy（检测政策，0 到 3 级严格程度）
   分析目标:
   检测阳性率随着检测政策升级是否下降。
   假设: 更严格的检测政策增加检测覆盖范围，从而降低阳性率，提升疫情控制效果。

5. 死亡人数 vs. 疫苗接种政策

   疫情指标: new_deaths_per_million（每百万人新增死亡数）
   政策: H7_Vaccination policy（疫苗接种政策，0 到 5 级严格程度）
   分析目标:
   分析疫苗接种政策推行后的新增死亡数变化。
   假设: 广泛的疫苗接种显著降低重症和死亡率。

ps: 指标数据集 `owid-covid-data.csv`, 政策数据集 `OxCGRT_compact_national_v1.csv`

## Wang Sen

1. 竖轴 new_deaths_per/new_case 横轴时间 折线图

2. 竖轴 new_deaths_per_million 横轴 people_vaccinated_per_hundred

3. 竖轴 icu_patients_per_million 横轴 people_vaccinated_per_hundred

4. new_death 中各种疫苗接种状态的对比

5. new_case 中各种疫苗接种状态对比

6. 竖轴 new_case_per_minllon 横轴 new_tests_smoothed_per_thousand
