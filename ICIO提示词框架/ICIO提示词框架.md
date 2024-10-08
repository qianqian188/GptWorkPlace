# ICIO提示词框架简介

## ICIO框架简介

### 要素：

#### 	1、Instruction 指令：执行的具体任务。

​		指令应该简洁、明确，确保AI模型能够理解任务的目标和要求。

#### 	2、Context 背景信息：提供背景信息，以引导模型生成更符合需求的回复。

​		背景信息可以包括任务的背景、目的、相关知识和其他相关信息

#### 	3、Input Data 输入数据：需要处理的数据。

​		在ICIO框架中，输入数据是可选的，如果AI模型不需要特定的输入数据，这一部分可以省略

#### 	4、Output Indicator 输出引导：告知所需输出的类型或风格。

​		它告诉模型如何组织和呈现响应结果。输出指示器应该与任务的需求相匹配，确保模型能够提供正确、有用的结果



### 适用范围：

#### 1、文本生成

​	请根据以下信息撰写一篇关于环保的重要性的文章。近年来，全球变暖和环境污染问题日益严重，各国政府和组织正在采取措施来应对这些挑战，但公众的意识和参与度仍然不足。关注点包括塑料污染、碳排放和可再生能源的使用，字数要求约500字。请以清晰、引人入胜的方式撰写，确保包括具体数据和例子，结尾提出个人可以采取的行动。

**拆解：**

​	**引导（I）**： “请根据以下信息撰写一篇关于环保的重要性的文章。”

​	**上下文（C）**： “近年来，全球变暖和环境污染问题日益严重。各国政府和组织正在采取措施来应对这些挑战，但公众的意识和参与度仍然不足。”

​	**输入（I）**： “关注点：塑料污染、碳排放、可再生能源的使用。字数要求：约500字。”

​	**输出（O）**： “请以清晰、引人入胜的方式撰写，确保包括具体数据和例子，结尾提出个人可以采取的行动。”

#### 2、数据分析

​	请分析销售数据，找出2024年第一季度的销售趋势和异常。我们提供的数据表包含产品名称、类别、销售额和销售日期。请生成一份报告，包含趋势图表和对异常销售额的解释。

**拆解：**

**引导（I）**：分析销售数据，找出季度销售趋势和异常。

**上下文（C）**：我们有2024年第一季度的销售数据，包含不同产品类别和地区的销售额。

**输入（I）**：提供的数据表包括产品名称、类别、销售额和销售日期。

**输出（O）**：生成一份报告，包含趋势图表和对异常销售额的解释。

#### 3、教育培训

​	请为初学者设计一个关于基础编程的课程大纲。课程目标是让学生掌握Python编程的基本概念和技能，适合没有编程经验的学习者。学生每周有3小时的学习时间，课程包括理论学习和实践练习。请提供一个为期四周的课程大纲，每周包括学习目标、主题和实践活动。

**拆解：**

**引导（I）**： 请为初学者设计一个关于基础编程的课程大纲。

**上下文（C）**： 课程目标是让学生掌握Python编程的基本概念和技能，适合没有编程经验的学习者。

**输入（I）**： 学生每周有3小时的学习时间，课程包括理论学习和实践练习。

**输出（O）**： 提供一个为期四周的课程大纲，每周包括学习目标、主题和实践活动。



#### 4、产品描述

​	请撰写一段关于新款智能手表的吸引性产品描述。这款手表具有健康监测、GPS导航和多种运动模式，适合活跃生活方式的用户。目标受众为健身爱好者，预算在200-300美元之间。生成的描述应在150字以内，突出手表的独特功能和使用场景。

**拆解：**

**引导（I）**：请撰写一段关于新款智能手表的吸引性产品描述。

**上下文（C）**：这款手表具有健康监测、GPS导航和多种运动模式，适合活跃生活方式的用户。

**输入（I）**：目标受众为健身爱好者，预算在200-300美元之间。

**输出（O）**：生成的描述应在150字以内，突出手表的独特功能和使用场景。
