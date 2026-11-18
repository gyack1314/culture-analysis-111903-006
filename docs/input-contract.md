# 合成分析资料契约

所有机构、企业、受访者、交易和事件均为本地合成，不来自新闻所涉真实主体，不声称新闻发生过这些分析问题。

seed.json与同名Parquet是相同原始值的两种载体；actions.json列尚未应用的后续输入动作。inventory.json只记录原件物理摘要和行数，不提供分析结论。时间均含时区或明确日期，金钱字段minor以CNY分计，空值保留未知含义。已有代码只做物理完整性检查，没有估计、预测、方案求解或产品发布功能。

lines以order/line标识原销售，bundle_parent指向同篮套装行；component是拆行展示，不再独立叠加父行金额或次数。gift和paid分开，basket_id为一次结算，household不是篮键。after_sales有return/exchange，指向明确原行，quantity为正，replacement_line仅为换出新品引用，不新增结算篮。availability逐商品展区日声明有售/缺货/未上架，缺记录为未知；eligible_basket分母需与商品共同可售范围一致。catalog分family/substitute_group与valid_from/to，licenses限定目标场次组合，packaging给体积与容量，margin以分计。discovery/confirmation是预先划定的不交叠展期，不能从确认期再选阈值并宣称独立验证。
