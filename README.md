# alist-毛玻璃美化
一个重度毛玻璃爱好者的alist美化
# 自定义头部
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="网站描述">
<meta name="keywords" content="网站关键词">
<meta name="robots" content="index, follow">
<meta property="og:site_name" content="网站名称">
<meta property="og:image" content="网站logoURL">
<!--Alist V3建议添加的，已经默认添加了，如果你的没有建议加上-->  
<script src="https://polyfill.alicdn.com/v3/polyfill.min.js?features=String.prototype.replaceAll"></script>
<!-- 引入图标-->
<link rel="stylesheet" href="https://cdn.bootcdn.net/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
  /*去掉底部*/
  .footer {
    display: none !important;
  }
  /*白天背景图*/
  .hope-ui-light {
    background-image: url("背景图url") !important;
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
    background-position-x: center;
  }
  /*夜间背景图*/
  .hope-ui-dark {
    background-image: url("背景url") !important;
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
    background-position-x: center;
  }
  /*主列表白天模式优化*/
  .obj-box.hope-stack.hope-c-dhzjXW.hope-c-PJLV.hope-c-PJLV-igScBhH-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*主列表夜间模式优化*/
  .obj-box.hope-stack.hope-c-dhzjXW.hope-c-PJLV.hope-c-PJLV-iigjoxS-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*readme白天模式优化*/
  .hope-c-PJLV.hope-c-PJLV-ikSuVsl-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;    
  }
  /*readme夜间模式优化*/
  .hope-c-PJLV.hope-c-PJLV-iiuDLME-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*顶部右上角切换按钮优化*/
  .hope-ui-light .hope-c-ivMHWx-hZistB-cv.hope-icon-button {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  .hope-ui-dark .hope-c-ivMHWx-hZistB-cv.hope-icon-button {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*右下角侧边栏按钮优化*/
  .hope-ui-light .hope-c-PJLV-ijgzmFG-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  .hope-ui-dark .hope-c-PJLV-ijgzmFG-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*白天模式代码块优化*/
  .hope-ui-light pre {
   background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*夜间模式代码块优化*/
  .hope-ui-dark pre {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*左侧侧边栏目录优化*/
  /*白天模式*/
  .hope-ui-light .hope-c-PJLV-ieGWMbI-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  }
  /*夜间模式*/
  .hope-ui-dark .hope-c-PJLV-ieGWMbI-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
  } 
  /* 返回顶部 */
  .hope-c-PJLV-ihVEsOa-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
    padding: var(--hope-space-1)!important;
  }
  .hope-ui-dark .hope-c-PJLV-ihVEsOa-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
    padding: var(--hope-space-1)!important;
}
  /*顶部*/
  #root > .header {
    background: rgba(255, 255, 255, 0);
  }
  /*导航条优化*/
  /*白天模式*/
  .hope-ui-light .body > .nav {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
    padding: var(--hope-space-1)!important;
    border-radius: var(--hope-radii-xl);
  }
  /*夜间模式*/
  .hope-ui-dark .body > .nav {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
    padding: var(--hope-space-1)!important;
    border-radius: var(--hope-radii-xl);
  }
  /*隐藏导航条遮罩*/
  .body > .nav::after {
    display: none;
  }
/* markdown链接优化 */
.markdown-body a {
    color: #06caeb!important;
    text-decoration: none;
}
/* 字体优化 */
* {
  font-weight: bold;
}
/*白天模式 搜索优化*/
.hope-ui-light .hope-c-PJLV-iiBaxsN-css{
   background-color: rgba(255,255,255,0.2)!important;
   backdrop-filter: blur(10px)!important;
}
  
/*白天模式 搜索栏优化*/
.hope-ui-light .hope-c-kvTTWD-hYRNAb-variant-filled{
   background-color: rgba(255,255,255,0.2)!important;
   backdrop-filter: blur(10px)!important;
}

/*白天模式 搜索优化*/
.hope-ui-light .hope-c-PJLV-ikEIIxw-css{
   background-color: rgba(255,255,255,0.2)!important;
   backdrop-filter: blur(10px)!important;
   padding: var(--hope-space-1)!important;
}

/*夜间模式搜索优化*/
.hope-ui-dark .hope-c-PJLV-iiBaxsN-css{
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
}

/*夜间模式搜索栏优化*/
.hope-ui-dark .hope-c-kvTTWD-hYRNAb-variant-filled{
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
}

/*夜间模式 搜索按钮优化*/
.hope-ui-dark .hope-c-PJLV-ikEIIxw-css{
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
    padding: var(--hope-space-1)!important;
}
/* 工具栏优化 */
.hope-c-iPJpIL-bVSmjq-size-xs {
    max-width: var(--hope-sizes-xs);
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
}
/* 搜索美化 */
.hope-c-PJLV-ihYBJPK-css {
  display: none!important;
}
.hope-c-PJLV-ihsROON-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
}
/* 公告美化 */
.hope-c-PJLV-ikJQsXT-css {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
}
/* 优化 */
.hope-c-zbPwS {
    background-color: rgb(255 255 255 / 10%)!important;
    backdrop-filter: blur(10px)!important;
}
</style>

# 自定义内容
<!--延迟加载-->  
<!--如果要写自定义内容建议都加到这个延迟加载的范围内-->  
<div id="customize" style="display: none;">
    <div>
     <br />
        <center class="dibu">
            <div style=" line-height: 19px;font-size: 14pt;font-weight: bold;">
            </div>  

            <div style="font-size: 16px; font-weight: bold;">
                <span class="nav-item">
                    <a class="nav-link" href="https://t.me/xxx"
                        target="_blank">
                        <i class="fa fa-telegram" aria-hidden="true"></i>
                        点击前往TG群聊 |
                    </a>
                </span>
                <span class="nav-item">
                    <a class="nav-link" href="xxxurl" target="_blank">
                        <i class="fa fa-envelope-open" aria-hidden="true"></i>
                        邮箱 |
                    </a>
                </span>
                <span class="nav-item">
                    <a class="nav-link" href="/@manage" target="_blank">
                        <i class="fa fa-cog" aria-hidden="true"></i>
                        管理 |
                    </a>
                </span>
                <span class="nav-item">
                    <a class="nav-link" href="https://github.com/Xhofe/alist" target="_blank">
                        <i class="fa fa-github" aria-hidden="true">
</i>
                        Alist
                    </a>
                </span>
	<br />
     <span class="nav-item">
          <a class="nav-link" href="https://icp.gov.moe/?keyword=xxx" target="_blank">
             <i class="fa fa-heart" aria-hidden="true"></i>
                萌ICP备xxx号
                </a>
            <span/>
        <br />
       <p>本站已存活 <span id="days">0</span> 天</p>
        <script>
            // 获取网站启动日期
            const launchDate = new Date("2024-0x-0x"); // 替换为你的网站启动日期

            // 计算运行天数
            const now = new Date();
            const diffTime = now - launchDate;
            const diffDays = Math.floor(diffTime / (1000 * 60 * 60 * 24));

            // 显示运行天数
            document.getElementById("days").textContent = diffDays;
        </script>
</script>
<!--延迟加载范围到这里结束-->
</div>
<!--延迟加载配套使用JS-->
<script>
    let interval = setInterval(() => {
        if (document.querySelector(".footer")) {
            document.querySelector("#customize").style.display = "";
            clearInterval(interval);
        }
    }, 200);
</script>
</script>
