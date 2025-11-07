<template>
  <!-- 
  ==============================================
  📌 关于我页面 - About Page
  ==============================================
  这个页面用来展示更详细的个人信息
  包括：个人介绍、技能展示、照片墙等
  
  💡 px-6 表示左右内边距为 6 单位，让内容不要紧贴边缘
  -->
  <div class="px-6">
    <!-- 
    ==============================================
    👤 个人介绍区域
    ==============================================
    包含 emoji 表情、姓名和一句话介绍
    -->
    <div class="mb-8">
      <!-- 
      ❗️ 修改表情符号：
      直接修改 emoji，可以从这里复制：https://emojipedia.org/
      常用 emoji: 👨‍💻 👩‍💻 🎓 🚀 ⚡ 🌟 💡
      -->
      <div class="text-6xl mb-4">🧑‍💻</div>

      <!-- 
      ❗️ 修改姓名：
      直接修改 <h2> 标签中的文字
      可以是中文、英文或中英文结合
      -->
      <h2 class="text-4xl font-bold text-gray-800">李乐祺 Lucky Lee</h2>

      <!-- 
      ❗️ 修改个人简介：
      在 <p> 标签中写一句话介绍自己
      可以包括：学校、专业、年级、兴趣爱好等
      -->
      <p class="text-xl text-gray-600">宁波诺丁汉大学数学与应用数学系大二学生。</p>

      <!-- 社交媒体链接 -->
      <div class="mt-4 flex gap-4">
        <a
          href="https://space.bilibili.com/你的ID"
          target="_blank"
          class="text-gray-600 hover:text-pink-500 transition-colors"
        >
          <Icon icon="ri:bilibili-fill" class="text-2xl" />
        </a>
        <a
          href="https://www.xiaohongshu.com/你的ID"
          target="_blank"
          class="text-gray-600 hover:text-red-500 transition-colors"
        >
          <Icon icon="ri:book-2-fill" class="text-2xl" />
        </a>
      </div>
    </div>

    <!-- 
    ==============================================
    ⭐ 技能展示区域
    ==============================================
    使用 Row 组件横向排列你的技能标签
    
    💡 Row 组件说明：
    - Row 用于水平排列内容
    - align="left" 表示内容靠左对齐
    - 也可以改为 align="center" 居中，或 align="right" 靠右
    -->
    <div class="mb-16">
      <h3>我的最爱</h3>

      <Row align="left">
        <div class="text-center w-32 bg-gray-50 rounded-lg p-4 hover:bg-gray-100 transition-colors">
          <div class="text-2xl mb-2">🎬</div>
          <p class="text-gray-700 font-medium">星际穿越</p>
          <p class="text-sm text-gray-500">最爱的电影</p>
        </div>
        <div class="text-center w-32 bg-gray-50 rounded-lg p-4 hover:bg-gray-100 transition-colors">
          <div class="text-2xl mb-2">🎵</div>
          <p class="text-gray-700 font-medium">港乐</p>
          <p class="text-sm text-gray-500">最爱的音乐</p>
        </div>
        <div class="text-center w-32 bg-gray-50 rounded-lg p-4 hover:bg-gray-100 transition-colors">
          <div class="text-2xl mb-2">🏸</div>
          <p class="text-gray-700 font-medium">羽毛球</p>
          <p class="text-sm text-gray-500">最爱的运动</p>
        </div>
      </Row>
    </div>

    <!-- 
    ==============================================
    � 座右铭区域
    ==============================================
    展示激励自己的座右铭
    -->
    <div class="mb-16">
      <h3>座右铭</h3>
      <div class="mt-4 p-6 bg-gray-50 rounded-lg border border-gray-100 shadow-sm">
        <p class="text-lg text-gray-700 italic">"生活不止眼前的苟且，还有诗和远方。"</p>
        <p class="mt-2 text-right text-gray-500">——北岛</p>
      </div>
    </div>

    <!-- 
    ==============================================
    �📷 照片墙区域
    ==============================================
    展示你的生活照片或作品集
    
    ❗️ 修改图片方法 1：使用在线图片
    将 src 中的网址替换成你的图片地址
    
    ❗️ 修改图片方法 2：使用本地图片
    1. 将图片拖到 src/assets 文件夹
    2. 修改 src，例如：src="/src/assets/photo1.jpg"
    
    💡 添加更多图片：
    复制 <img> 这一行，粘贴在下面，然后修改图片地址
    
    💡 调整图片大小：
    修改 class 中的 w-5/12
    - w-3/12: 占 25% 宽度（更小）
    - w-5/12: 占 42% 宽度（中等）
    - w-6/12: 占 50% 宽度（一半）
    - w-full: 占 100% 宽度（全宽）
    -->
    <div class="mb-16">
      <h3>照片</h3>
      <Row align="left">
        <img src="https://picsum.photos/300/200?random=1" class="rounded-lg shadow-md w-5/12" />
        <img src="https://picsum.photos/300/200?random=2" class="rounded-lg shadow-md w-5/12" />
      </Row>
    </div>
  </div>
</template>
