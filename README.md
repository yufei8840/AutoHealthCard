# AutoHealthCard
![auto_health_card](https://github.com/Jasonzj/AutoHealthCard/workflows/auto_health_card/badge.svg)

吉珠自动填写健康卡

## Usage:

### Method 1: 
1. Create a new repository
2. Copy the .github directory to your own repository
3. Set the [Secrets](#Secrets)

### Method 2 (Recommended):
1. Fork this repository
2. In your forked repository
3. Set the [Secrets](#Secrets)
5. Configure [Pull](https://github.com/wei/pull) to update your repository whenever upstream updates.

The action will automatically run at 10 and 11am(GMT+8) everyday.

## Secrets
|name|description|
|---|---|
|SCKEY|server酱|
|USERNAME||
|PASSWORD||
|RANGE|student id range<br>`04181101:04181120`<br>support multiple ranges<br>`04181101:04181110,04182201:04182215`|
|LIMIT|concurrence limit<br>default value is 1|

This repository has two different mode scripts that sign-in, one is browser mode and the other is request mode.

Set `USERNAME` and `PASSWORD` will run **browser mode** by default.

Continuing to set `RANGE` and `LIMIT` will enable **request mode**. 

> Notice: if the RANGE difference is greater than 10, the log will not be pushed to WeChat 

