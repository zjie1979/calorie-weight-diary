# 轻记热量

中文移动端 PWA：食物重量与热量、每日消耗、体重、三天均值、累计缺口估算。纯静态页面，无账号、无追踪、无远程数据库；个人记录仅存于浏览器 localStorage。

计算：三天窗口含所选日及前两天，有食物或标记完成的日期参与摄入平均，填写体重的日期参与体重平均；缺失日期不当成零。累计缺口只包含起始日至所选日期间，饮食完成且填了消耗的日期。预估体重（斤）= 起始体重 − 净缺口 / 3000。此比例为使用者指定的简化模型，不是实际减重承诺。

GitHub Pages 发布 main 分支根目录。Safari 打开 → 分享 → 添加到主屏幕。支持离线缓存、食物修改删除、日期补录、JSON 备份导出与合并导入。更换浏览器、设备或域名不会自动迁移记录。

体重实际变化受水分、代谢等影响，参考 NIH：https://www.niddk.nih.gov/research-funding/at-niddk/labs-branches/laboratory-biological-modeling/integrative-physiology-section/research/body-weight-planner
