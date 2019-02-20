## Welcome to DJ's bolg
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>钟表</title>
        <script type="text/javascript">
            function getDou(number) {
                if(number < 10) {
                    return '0' + number;
                } else {
                    return number;
                }
            }

            function getWeek(week) {
                var sWeek = null;
                switch(week) {
                    case 0:
                        sWeek = '星期日'
                        break;
                    case 1:
                        sWeek = '星期一'
                        break;
                    case 2:
                        sWeek = '星期二'
                        break;
                    case 3:
                        sWeek = '星期三'
                        break;
                    case 4:
                        sWeek = '星期四'
                        break;
                    case 5:
                        sWeek = '星期五'
                        break;
                    case 6:
                        sWeek = '星期六'
                        break;
                    default:
                        break;
                }
                return ' ' + sWeek;
            }
            window.onload = function() {
                var oDate = document.getElementsByTagName("p")[0];
                var oTime = document.getElementsByTagName("p")[1];

                function tick() {
                    var date = new Date();
                    var sDate = null;
                    var sTime = null;
                    var hours = date.getHours();
                    if(hours > 12) {
                        hours %= 12;
                        sTime = '下午 ';
                    } else {
                        sTime = '上午 ';
                    }
                    sTime += getDou(hours) + ':' + getDou(date.getMinutes()) + ':' + getDou(date.getSeconds());
                    sTime += getWeek(date.getUTCDay());
                    oTime.innerHTML = sTime;

                    sDate = date.getUTCFullYear() + "年";
                    if(date.getUTCMonth() < 9) {
                        sDate += '0' + (date.getUTCMonth() + 1) + "月";
                    } else {
                        sDate += (date.getUTCMonth() + 1) + "月";
                    }
                    sDate += date.getUTCDate() + "日";
                    oDate.innerHTML = sDate;
                }

                setInterval(tick, 1000);
                tick();
            }
        </script>
        <style type="text/css">
            body {
                width: 200px;
                height: 200px;
                background: #323332;
                vertical-align: middle;
                display: table-cell;
            }

            .date {
                text-align: center;
                color: yellow;
                font-size: 30px;
            }

            .time {
                text-align: center;
                color: yellow;
                font-size: 30px;
            }
        </style>
    </head>
    <body>
        <div>
            <p class="date">
                日期
            </p>
            <p class="time">
                时间
            </p>
        </div>
   




<audio autoplay="autoplay" height="100" width="100">
  <source src="小果 - 蒲公英的梦想.mp3" type="audio/mp3" />
  <source src="小果 - 蒲公英的梦想.ogg" type="audio/ogg" />
  <embed height="100" width="100" src="小果 - 蒲公英的梦想.mp3" />
</audio>
     </body>
</html>


