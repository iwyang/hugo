---
title: "说说"
slug: "say"
toc: false
menu:
    main:
        name: 说说 
        weight: -80
        params: 
            icon: say
edit: false
comments: false
---
## 说说
<style>
.article-header {
    display: none;
  }
</style>

<div class="js-pjax" id="tip" style="text-align:center;">ipseak加载中</div>
<div class="js-pjax" id="ispeak"></div>
<link
  rel="stylesheet"
  href="https://cdn.staticfile.org/highlight.js/10.6.0/styles/atom-one-dark.min.css"
/>
<link
  rel="stylesheet"
  href="https://cdn1.tianli0.top/npm/ispeak@4.3.2/style.css"
/>

<style>
  #article-container .D-avatar {
    margin: 0 10px 0 0;
  }
  .D-footer {
    display: none;
  }
</style>
<script src="https://cdn.staticfile.org/highlight.js/10.6.0/highlight.min.js"></script>
<script src="https://cdn.staticfile.org/marked/2.0.0/marked.min.js"></script>
<script src="https://cdn1.tianli0.top/npm/discuss@1.1.4/dist/discuss.js"></script>
<script src="https://cdn1.tianli0.top/npm/ispeak@4.3.2/ispeak.umd.js"></script>
<script>
  var head = document.getElementsByTagName('head')[0]
  var meta = document.createElement('meta')
  meta.name = 'referrer'
  meta.content = 'no-referrer'
  head.appendChild(meta)
  if (ispeak) {
    ispeak
      .init({
        el: '#ispeak',
        api: 'https://kkapi-dev.vercel.app/',
        author: '61fe93508fd621d39a155725',
        pageSize: 10,
        loading_img: 'https://bu.dusays.com/2022/05/01/626e88f349943.gif',
        speakPage: '/say',
        githubClientId: 'Iv1.c90b52a4e197df3c',
        initCommentName: 'discuss',
        initCommentOptions: {
          serverURLs: 'https://discuss-umber.vercel.app/'
        }
      })
      .then(function () {
        console.log('ispeak 加载完成')
        document.getElementById('tip').style.display = 'none'
      })
  } else {
    document.getElementById('tip').innerHTML = 'ipseak依赖加载失败！'
  }
</script>