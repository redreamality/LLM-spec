# LLM-spec
大模型需求规格说明书模板

〔为每个确定的商业功能（需实现的功能）描述其定义、业务规则，详细叙述如何从输入转变到输出并且如何获得、处理和产生这些信息。这些内容在下列标题中有条理的阐述。


1. 业务定义/描述/目的。主要的功能是什么？开发程序的原因是什么？适用的用户类型？
2. 环境。程序与哪些内外部系统交互？有哪些前置依赖？提供哪些接口？
    1. 前置依赖：依赖哪些
    2. 前置条件。在执行本功能前需要完成的前置条件。
        1. 鉴权：指用户操作本功能所需的授权。
        2. 数据依赖：指为了完成该功能所必须的文档/数据库/多模态内容等。
        3. 配置
    3. 外部接口包括：硬件接口、软件接口、通信接口，每个接口需考虑以下内容：
        1. 接口描述，包括接口类型、接口特点（如版本、名称、来源等）
        2. 接口与本系系统的输入输出关系
        3. 技术方面的约束
        4. 转换的安全考虑
3. 业务规则/业务要素/业务专业术语解释。
4. 功能内涵：精确地阐述它做了什么。
    1. 页面类需求：功能项的主要页面样式和跳转逻辑。
    2. 算法类需求：
5. 约束、限制与特殊考虑
    1. 哪些已知情况下，程序默认不做处理。
    2. 有哪些会导致程序运行异常的情况？这些异常会抛出什么样的报错信息？
    3. 列出当前方案下功能的限制并提供其原因。
    4. 其他任何必要的特殊考虑。
6. 输入一输出的形式化定义：提供所有与本功能有关的输入、输出描述，包括但不限：输入/输出数据类型、媒体、格式、数值范围、精度、单位等。
7. 范围。
    1. 辅助资料的范围是什么？主程序能够使用的内容，包括但不限于：知识库、工具插件等。
    2. 输入的有效范围是什么？这一部分通过测试集体现。测试数据集写出具体路径。
8. 验收指标：判断功能已经完整实现的依据。期望结果的效果是什么？效果如何度量？
    1. 页面类：测试用例
    2. 算法类：测试数据集上的效果指标。
9. 业务操作流程/实现功能/使用的算法：描述正常业务流程，列举异常情况和处理流程。建议使用图示，并配合必要的文字说明
10. 选项。用户的功能选项有哪些？如何在选项之间进行挑选？
11. 独立于总体要求的非功能需求（包括但不限于时间要求，并发要求等，参见4.1）
    1. 设计并发数。
    2. 运行时间要求。在指定的配置下，解决特定规模问题所需要的时间？包括：平均运行时间，90%情况下的最大运行时间。
