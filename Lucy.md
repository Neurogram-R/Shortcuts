# Lucy
Lucy is a fully customizable smart (voice) assistant shortcut that leverages the actions provided by [ChatGPT](https://apps.apple.com/us/app/id6448311069) to integrate with actions from other apps or APIs. You can freely combine different functionalities for Lucy to assist you in accomplishing various daily tasks.

## Manual
 - [English](https://neurogram.notion.site/Lucy-3436b58b7edd4368bcfe0ced41006a10)
 - [简体中文](https://neurogram.notion.site/Lucy-8492b0a0ff73481ba1a8d5a922cbd490)

## Download
 - [Lucy](https://www.icloud.com/shortcuts/3ff326defcee44f69ad0af40f4b62c63)
 - [Lucy](https://www.icloud.com/shortcuts/312f819577b6416c978addec844ebf3b) (简体中文)

## Plugins
| Name | App | Intro | Prompts | 
| ---- | ---- | ---- | ---- |
| [Reminders GPT](https://www.icloud.com/shortcuts/dbdc4b17e8454cd8a1cb7260f5145110) | [Reminders](https://apps.apple.com/us/app/reminders/id1108187841) | querying, adding, and editing reminders<br>查询、添加、编辑提醒事项 | [Check](#reminders-gpt) |
| [Weather GPT](https://www.icloud.com/shortcuts/1f20c4617584493397a1b7c8a77a3968) | [Weather](https://apps.apple.com/us/app/id1069513131) |querying weather information<br>查询天气信息 | [Check](#weather-gpt) |



## Plugins Prompts

### Reminders GPT
```
# English

Get reminders, to-dos, schedule
Params:
 - method*: get_reminders
 - shortcuts*: Reminders GPT

Add reminders, to-dos, schedule
Params:
 - method*: add_reminders
 - shortcuts*: Reminders GPT
 - title*: the appropriate title for the event
 - notes: Details or notes for the event
 - date: specific event time or "anytime". Time format should be yyyy-MM-dd hh:mm:ss

Edit reminders, to-dos, schedule
Params:
 - method*: edit_reminders
 - shortcuts*: Reminders GPT
 - id*: the unique ID of the event (can be obtained through the get_reminders method)
 - title*: the appropriate title for the event
 - notes: Details or notes for the event
 - date: specific event time or "anytime". Time format should be yyyy-MM-dd hh:mm:ss


# 简体中文

获取提醒事项、待办事项、日程安排
参数：
 - method*：get_reminders
 - shortcuts*：Reminders GPT

添加提醒事项、待办事项、日程安排
参数：
 - method*：add_reminders
 - shortcuts*：Reminders GPT
 - title*：符合事件内容的标题
 - notes：事件的详细信息或备注
 - date：具体的事件时间或"anytime"。时间格式应为 yyyy-MM-dd hh:mm:ss

编辑提醒事项、待办事项、日程安排
参数：
 - method*：edit_reminders
 - shortcuts*：Reminders GPT
 - id*：事件的唯一 ID（可通过 get_reminders 方法获取）
 - title*：符合事件内容的标题
 - notes：事件的详细信息或备注
 - date：具体的事件时间或"anytime"。时间格式应为 yyyy-MM-dd hh:mm:ss
```

### Weather GPT
```
# English

Get the current weather
Params:
 - method*: get_weather
 - shortcuts*: Weather GPT


# 简体中文

获取当前天气
参数：
 - method*：get_weather
 - shortcuts*：Weather GPT
```
