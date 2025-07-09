# AICGSecEval Evaluation Results Upload

This repository contains records of submissions to the AICGSecEval leaderboard.

## 🏆 Participate in the Leaderboard
To evaluate your model using AICGSecEval, please refer to the instructions in the [main repository](https://github.com/Tencent/AICGSecEval).

Please follow the instructions carefully to ensure your submission is merged in a timely manner!

1. Fork the current repository.
2. Create a new folder under the `evaluation` directory, naming it with your model name and submission date (e.g., your_model_name_20250720).
3. In the newly created folder (`evaluation/your_model_name_20250720/`), provide the following data:
    > The following content is automatically generated during the AICGSecEval evaluation process, with the default path being `outputs/generated_code/{model_name}__{batch_id}/`
    * `eval_result.json`
    * `processed_instances.json`
    * `sast_results.json`
    * `sast_results/` directory, containing all files with the suffix `_output.json`
    * All patch files generated during the evaluation process, preserving the original directory structure (e.g., `sqli_02_cycle2/patch.diff`)
        * Note: Only keep `patch.diff` files and delete other unrelated files in the directory.
        * If no `patch.diff` files are found in a directory, you can check the corresponding `backup` directory (e.g., `sqli_02_cycle2_backup`) for them.

## ✅ Result Verification

If you are interested in receiving the "verified" checkmark on your submission, please do the the following:

1. Create an Issue
2. In the Issue, provide instructions on how to run your model.
3. We will run local tests on your model and verify the results.

