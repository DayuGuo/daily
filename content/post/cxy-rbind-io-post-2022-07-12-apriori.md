---
title: 基于关联规则的购物篮分析
date: '2022-07-12'
linkTitle: https://cxy.rbind.io/post/2022/07/12/apriori/
source: 首页 on 楚新元 | All in R
description: |-
  理解关联规则 购物篮分析主要用于超市数据。例如{尿布，婴儿食品，啤酒}在超市可能是一个典型的交易，该交易中识别的规则或许可以表示为如下形式{尿布，婴儿食品}-&gt;{啤酒}，换句话说，即“尿布和婴儿食品意味着啤酒”，这就是关联规则。
  度量规则兴趣度 关联规则最广泛使用的方法就是Apriori算法。关联规则是否是令人感兴趣的取决于三个统计量：支持度、置信度、提升度。下面举例说明。 交易号 购买的商品 1 {鲜花，慰问卡，苏打水} 2 {毛绒玩具熊，鲜花，气球，糖块} 3 {鲜花，慰问卡，糖块} 4 {毛绒玩具熊，气球，苏打水} 5 {鲜花，慰问卡，苏打水} 支持度（support）。support(X) = count(X) / N，以上交易数据中，{鲜花}的支持度为4/5=0.8，{鲜花，慰问卡}的支持度为3/5=0.6。鲜花和慰问卡同时购买的交易比数占整个交易比数的60%； ...
disable_comments: true
---
理解关联规则 购物篮分析主要用于超市数据。例如{尿布，婴儿食品，啤酒}在超市可能是一个典型的交易，该交易中识别的规则或许可以表示为如下形式{尿布，婴儿食品}-&gt;{啤酒}，换句话说，即“尿布和婴儿食品意味着啤酒”，这就是关联规则。
度量规则兴趣度 关联规则最广泛使用的方法就是Apriori算法。关联规则是否是令人感兴趣的取决于三个统计量：支持度、置信度、提升度。下面举例说明。 交易号 购买的商品 1 {鲜花，慰问卡，苏打水} 2 {毛绒玩具熊，鲜花，气球，糖块} 3 {鲜花，慰问卡，糖块} 4 {毛绒玩具熊，气球，苏打水} 5 {鲜花，慰问卡，苏打水} 支持度（support）。support(X) = count(X) / N，以上交易数据中，{鲜花}的支持度为4/5=0.8，{鲜花，慰问卡}的支持度为3/5=0.6。鲜花和慰问卡同时购买的交易比数占整个交易比数的60%； ...