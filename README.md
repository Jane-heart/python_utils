# python_utils
此处用于存放python通用的操作

## 当前仓库包含内容
common_utils：
    调用openAI的基本操作
    导入环境变量

## 使用示例
```python
import common_utils 

common_utils.import_env_variables([common_utils.OPENAI_API_KEY])

prompt = f"""
要求使用现在进行时的语法去修改下面内容：
Add import environment variables and call openAI methods
"""
response = common_utils.get_completion(prompt=prompt)

print(response)
```