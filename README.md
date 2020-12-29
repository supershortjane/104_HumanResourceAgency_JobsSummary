# 104_HumanResourceAgency_JobsSummary

## 1.Goal
爬梳104動態網站，並產出依特定關鍵字搜尋的工作職缺、工作內容、條件要求及技能統整的CSV檔<br/>
Web Craweld job information based on a specific keyeword on a popular Human Resource Agency in Taiwan 

## 2.Process
```
1.Observe the website
2.Web crawl the website
3.Export data
```  
## Observe the website
My finding:<br/>
◆ The request method is get.<br/>
◆ The website page is dynamic since as I roll down the page, the website show more jobs to me.<br/>
◆ The data that I want to crawl is in the url:https://www.104.com.tw/job/ajax/content/ and stored as json.<br/>

## Web crawl the website

The problem that I face when I am crawling:<br/>
Since some of job such as outsourcing jobs, tutoring jobs is linked to another websites which have different format, 
I decide that when my web crawler encounter the sites, it would pass and go to crawl the next one.

## Export data
I organize all the information into one table and save it as a csv file.
依"資料分析"關鍵字搜尋，產出結果檔示意如下:<br/>
The file is like:<br/>
![image](https://user-images.githubusercontent.com/32606310/100188409-16569300-2f25-11eb-921e-0a5ac557dfb6.png)

