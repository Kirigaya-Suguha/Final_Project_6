1. 政策严格指数与确诊/死亡数据对比---------多轴折线图
X轴：时间
Y轴1：政策严格指数（或者政策string）
Y轴2：每日新增确诊病例数（new_cases）或新增死亡数（new_deaths）
分析思路：
展示政策收紧或放松对新增病例和死亡人数的影响。
比较不同国家政策实施时间与疫情控制效果的差异


2. 累计病例/死亡与疫苗接种的关系----------散点图
X轴：累计接种疫苗剂次占比（people_vaccinated_per_hundred）
Y轴：累计确诊病例（total_cases）或累计死亡人数（total_deaths）
分组：国家
分析思路：
探讨疫苗接种覆盖率与疫情严重程度的关系。比较疫苗接种速度对疫情减缓的影响。


3. 经济发展与疫情严重程度-----散点图
X轴：gdp_per_capita
Y轴：total_cases_per_million 或 total_deaths_per_million
分析思路：
观察经济发达国家是否更容易减少死亡率或确诊率。


4. 医疗资源与死亡率的关系-----散点图
图表类型：散点图或气泡图（每千人医院床位数）
X轴：hospital_beds_per_thousand
Y轴：total_deaths_per_million
分析思路：
观察医疗资源是否影响疫情中死亡人数的多少。


5. 健康水平与疫情传播的关系----散点图或线性回归图
问题：健康水平较高的国家是否更能控制疫情？
分析方法：
X轴：life_expectancy（人均预期寿命）
Y轴：total_cases_per_million 或 reproduction_rate（疫情传播速度）
分析思路：
长寿通常与良好的医疗系统和健康水平相关，可能影响疫情传播速度和确诊率。
验证是否健康水平较高的国家，疫情更容易被控制。
