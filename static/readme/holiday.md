 #### 2018-11-22
 #### 节假日管理 版本1.0.0
1.节假日查询接口访问

  1.1 查询指定日期是否是节假日请求方式 http://IP:PORT/holidayCheck?date=yyyyMMdd
    
        yyyyMMdd： 日期格式：年月日 如: 20181126
        
   e.g.
        [http://10.100.147.39:8080/holidayCheck?date=20181126](http://10.100.147.39:8080/holidayCheck?date=20181126)
       
        响应结果:
               {
                 "retCode": "0000",
                 "retInfo": "获取成功",
                 "data": {
                    "isHoliday": false
                 }
               } 
               
    retCode "0000" 且 isHoliday false 时 当日不是节假日
    retCode "0000" 且 isHoliday true  时 当日是节假日
    retCode 不为"0000" 查询失败 请检查参数或重试
