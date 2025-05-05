### [👉👉👉♥♥点此进入♥观看入口👈👈👈](https://mrddrm.github.io/jizz.html)
<br></br><br></br><br></br>
user_data = self.users[self.current_user]
        metrics = user_data['health_metrics']
        
        end_date = datetime.datetime.now().date()
        start_date = end_date - datetime.timedelta(days=days-1)
        
        filtered_metrics = [
            m for m in metrics 
            if m['type'] == metric_type and 
               datetime.datetime.strptime(m['date'], '%Y-%m-%d').date() >= start_date
        ]
        
        # 按日期排序
        filtered_metrics.sort(key=lambda x: x['date'])
        
        dates = [m['date'] for m in filtered_metrics]
        values = [m['value'] for m in filtered_metrics]
