<!DOCTYPE html>
<html lang="en"><head>
    <meta charset="UTF-8">
    <title>小傻子</title>
    <script src="http://apps.bdimg.com/libs/jquery/2.1.4/jquery.min.js"></script>
    <link href="http://apps.bdimg.com/libs/bootstrap/3.3.4/css/bootstrap.min.css" rel="stylesheet">
    <script src="http://apps.bdimg.com/libs/bootstrap/3.3.4/js/bootstrap.min.js"></script>

    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
</head>
<body>
<div class="container">
    <div class="row col-md-3"></div>
    <div class="row col-md-6">
        <div class="row question">
            <div class="col-md-6 col-xs-12">
                <p style="line-height: 50px;font-size: 30px;">“<a href="123.com">小傻子，我观察你很久了”</a></p>
                <p style="line-height: 50px;font-size: 30px;">你是不是很傻啊，哈哈^v^！！</p>
            </div>
            <div class="col-md-6 col-xs-12">
                <img style="height: 100px;" alt="" src="https://p.upyun.com/demo/tmp/O39Xh5Z2.gif">
            </div>
        </div>
        <div class="row question" style="margin-top: 50px;">
            <div class="col-md-6 col-xs-6" style="text-align: center;">
                <button class="btn btn-success" id="no" style="width: 80%" type="button">是</button>
            </div>
            <div class="col-md-6 col-xs-6" style="text-align: center;">
                <button class="btn btn-danger" id="ok" style="width: 80%" type="button">不是</button>
            </div>
        </div>
        <div class="col-md-12 col-xs-12 hide" id="success">
            <img style="width: 100%;" alt="" src="https://p.upyun.com/demo/tmp/vPp5Y8hv.gif">
        </div>
    </div>

    <div class="row col-md-3"></div>

</div>
<script>
    var i=1;
    var ok=false;
    $(document).ready(function(){
        $("#no").click(function(){
            alert("真的啊，我就知道你是个傻子 哈哈^v^");
            alert("现在是不是很想知道我是谁，嘿嘿 我就不告诉你^v^");
            $(".question").addClass('hide');
            $("#success").removeClass('hide');
            ok=true;
        });
        $("#ok").click(function(){
            switch(i){
                case 1:
                    alert("不仅丑");
                    break;
                case 2:
                    alert("还那么胖");
                    break;
                case 3:
                    alert("名字又难听");
                    break;
				case 4:
                    alert("天天就知道吃");
                    break;
                case 5:
                    alert("还不知道减肥");
                    break;
                default:
                    alert("还不承认");
            }
            i++;
        });
    });
</script>

</body></html>
