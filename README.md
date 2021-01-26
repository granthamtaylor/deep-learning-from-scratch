# Example IPython Notebook Repository
This is an example repository with content that can be auto-updated (auto file PRs) into the Boulevard Insights portal.

## Process

1. Use this repository as a template and develop your code as you normally would.
2. Include the [workflow file](./.github/workflows/copy_ipynb.yml) and make sure to update the values of the following keys:
    - `paths`: update to match the path to the ipynb file that you want synced; this way this action is only triggered on changes to the article content and not any other changes to your source repository.
    - `src_path` (source path): update to match the path to the ipynb file that you want synced into the Boulevard Insights content section.
    - `dst_path` (destination path): update to match the file path to which you want your ipynb file copied in the Boulevard insights repository.
    - `commmit_message`: update to be specific to your notebook/article.
3. Once you push changes to your `main` branch on this repository, it will trigger a push to the [autoupdate-content](https://github.com/boulevardcg/insights_portal/tree/autoupdate-content) branch of the Boulevard Insights repository and a pull request will be automatically made to merge the updates with the [master](https://github.com/boulevardcg/insights_portal/tree/master) branch.
