# AICGSecEval 评测结果上传

该仓库包含提交到 AICGSecEval 排行榜的记录。


## 🏆 参与排行榜
使用 AICGSecEval 评估模型的方法请查看[主仓库](https://github.com/Tencent/AICGSecEval)中的说明。

请仔细按照这些说明操作，以确保您的提交能够及时合并！

1. Fork 当前仓库。
2. 在 `evaluation` 目录下创建新文件夹，使用模型名称和提交日期命名（例如：your_model_name_20250720）
3. 在创建的新文件夹 (`evaluation/your_model_name_20250720/`) 中提供如下数据：
    > 下列内容由 AICGSecEval 评测过程中自动生成，默认生成路径为 `outputs/generated_code/{model_name}__{batch_id}/`
    * `eval_result.json`
    * `processed_instances.json`
    * `sast_results.json`
    * `sast_results/` 目录，包含原目录下所有后缀为`_output.json`的文件
    * 评测过程中生成的所有补丁文件，保留原始目录结构，例如 `sqli_02_cycle2/patch.diff`
        * 注意仅保留 `patch.diff` 文件，删除目录下其他无关文件。
        * 若某目录下未发现 `patch.diff` 文件，可去对应的 `backup` 目录（例如`sqli_02_cycle2_backup`）寻找

## ✅ 结果验证

如果您有兴趣在您的提交中获得“已验证”标记，请按照以下步骤操作：

1. 创建一个 Issue
2. 在 Issue 中提供运行您模型的指令和方法。
3. 我们将对您的模型进行本地测试并验证结果。




