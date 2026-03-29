<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>智能聊天系统</title>
    <style>
        * {margin: 0;padding: 0;box-sizing: border-box;font-family: "Segoe UI", "Microsoft YaHei", sans-serif;}
        body {
            background: #f8f9fa;
            height: 100vh;
            display: flex;
            overflow: hidden;
            position: relative;
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            transition: background 0.3s;
        }
        .blur-bg {
            position: fixed;
            top:0;left:0;
            width:100%;height:100%;
            background: rgba(0,0,0,0.25);
            backdrop-filter: blur(12px);
            display: none;
            z-index:998;
        }
        .container {
            display: flex;
            width: 100%;
            height: 100%;
            position: relative;
            z-index:1;
        }
        .sidebar {
            width: 280px;
            background: rgba(255,255,255,0.92);
            border-right: 1px solid rgba(0,0,0,0.06);
            color: #2d3748;
            padding: 16px;
            display: flex;
            flex-direction: column;
            backdrop-filter: blur(10px);
            box-shadow: 2px 0 15px rgba(0,0,0,0.05);
        }
        .user-info {
            padding: 12px;
            border-bottom: 1px solid rgba(0,0,0,0.05);
            margin-bottom: 12px;
            position: relative;
            display: flex;
            align-items: center;
            gap:10px;
        }
        .avatar {
            width: 52px;
            height: 52px;
            border-radius: 50%;
            background: #ffffff;
            border: 1px solid #e2e8f0;
            overflow: hidden;
            flex-shrink: 0;
            cursor: pointer;
        }
        .avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .settings-btn {
            position: absolute;
            top:12px; right:10px;
            width:34px; height:34px;
            border-radius:50%;
            background: linear-gradient(135deg, #4299e1, #3182ce);
            color:white;
            display:flex; align-items:center; justify-content:center;
            cursor:pointer; font-size:16px; border:none;
            box-shadow: 0 3px 8px rgba(66,153,225,0.25);
            transition: 0.2s;
        }
        .settings-btn:hover {
            transform: scale(1.08);
        }
        .settings-menu {
            position: absolute;
            top: 50px; right: 10px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            width: 170px;
            padding: 6px 0;
            display: none;
            z-index: 100;
        }
        .settings-menu div {
            padding: 10px 14px;
            cursor: pointer;
            font-size: 14px;
            border-radius: 6px;
            margin: 2px 6px;
        }
        .settings-menu div:hover {
            background: #f7fafc;
        }
        .add-btn {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, #38a169, #2f855a);
            color: white;
            border: none;
            border-radius: 10px;
            margin: 10px 0;
            cursor: pointer;
            font-weight: 500;
            box-shadow: 0 3px 10px rgba(56,161,105,0.2);
            transition: 0.2s;
        }
        .add-btn:hover {
            transform: translateY(-1px);
        }
        .list {
            flex: 1;
            overflow-y: auto;
            padding-right: 4px;
        }
        .item {
            padding: 14px;
            border-radius: 10px;
            margin: 6px 0;
            cursor: pointer;
            background: rgba(247,250,252,0.8);
            transition: 0.2s;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .item:hover {
            background: #edf2f7;
            transform: translateX(2px);
        }
        .chat-box {
            flex: 1;
            display: flex;
            flex-direction: column;
            background: rgba(255,255,255,0.94);
            backdrop-filter: blur(10px);
        }
        .chat-title {
            padding: 16px 20px;
            border-bottom: 1px solid rgba(0,0,0,0.05);
            font-weight: 600;
            font-size: 16px;
            display:flex;
            justify-content:space-between;
            align-items:center;
        }
        .chat-menu {
            position: relative;
        }
        .menu-btn {
            font-size: 20px;
            background: none;
            border: none;
            cursor: pointer;
            padding: 4px 8px;
        }
        .menu-popup {
            position: absolute;
            top: 35px; right: 0;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            width: 150px;
            z-index: 100;
            display: none;
        }
        .menu-popup div {
            padding: 10px 14px;
            cursor: pointer;
            font-size: 14px;
        }
        .menu-popup div:hover {
            background: #f7fafc;
        }
        .msg-list {
            flex: 1;
            padding: 24px;
            overflow-y: auto;
            background: rgba(248,250,252,0.6);
        }
        .msg-row {
            display: flex;
            gap: 10px;
            margin: 10px 0;
            align-items: flex-end;
        }
        .msg-row.me {
            flex-direction: row-reverse;
        }
        .msg-avatar {
            width: 38px;
            height: 38px;
            border-radius: 50%;
            background: #ffffff;
            border: 1px solid #e2e8f0;
            overflow: hidden;
            flex-shrink: 0;
            cursor: pointer;
        }
        .msg-avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .msg {
            padding: 12px 16px;
            border-radius: 14px;
            max-width: 72%;
            line-height: 1.5;
            font-size: 15px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }
        .my-msg {
            background: linear-gradient(135deg, #4299e1, #3182ce);
            color: white;
            border-bottom-right-radius: 4px;
        }
        .other-msg {
            background: white;
            color: #2d3748;
            border-bottom-left-radius: 4px;
        }
        .file-msg {
            color: #fff;
            background: #2d3748 !important;
            cursor: pointer;
        }
        .input-box {
            display: flex;
            padding: 16px 20px;
            border-top: 1px solid rgba(0,0,0,0.05);
            background: white;
            gap: 10px;
        }
        #msg-input {
            flex: 1;
            padding: 12px 16px;
            border: 1px solid rgba(0,0,0,0.08);
            border-radius: 12px;
            outline: none;
            font-size: 15px;
            transition: 0.2s;
        }
        #msg-input:focus {
            border-color: #4299e1;
            box-shadow: 0 0 0 2px rgba(66,153,225,0.15);
        }
        .send-btn {
            padding: 12px 20px;
            background: linear-gradient(135deg, #4299e1, #3182ce);
            color: white;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            font-weight: 500;
            transition: 0.2s;
        }
        .send-btn:hover {
            transform: translateY(-1px);
        }
        .file-btn {
            padding: 12px;
            background: #718096;
            color: white;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            transition: 0.2s;
        }
        .modal {
            position: fixed;
            top: 50%; left: 50%;
            transform: translate(-50%,-50%);
            background: white;
            padding: 28px;
            border-radius: 16px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.12);
            display: none;
            z-index: 999;
            width: 90%;
            max-width: 380px;
        }
        .modal input {
            width: 100%;
            padding: 12px 14px;
            margin: 8px 0;
            border: 1px solid rgba(0,0,0,0.08);
            border-radius: 10px;
            font-size: 15px;
        }
        .modal button {
            padding: 11px 16px;
            background: #4299e1;
            color: white;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            margin-top: 6px;
            font-weight: 500;
        }
        .tip {
            font-size:13px;
            color:#dd6b20;
            margin-bottom:10px;
        }
        video#bgVideo {
            position:fixed;
            top:0; left:0;
            width:100%; height:100%;
            object-fit:cover;
            display:none;
            z-index:0;
        }
        #bgInputImg, #bgInputVideo, #avatarInput {display:none;}
        .close-btn {
            position: absolute;
            top: 16px;
            right: 20px;
            font-size: 20px;
            cursor: pointer;
            color: #718096;
        }
        .request-item {
            padding: 10px;
            background: #f7fafc;
            border-radius: 8px;
            margin: 6px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .request-btn {
            padding: 6px 10px;
            border-radius: 6px;
            border: none;
            cursor: pointer;
            font-size: 12px;
        }
        .agree {background: #38a169; color: white;}
        .refuse {background: #e53e3e; color: white;}

        /* 可拖动悬浮调试面板 */
        #devModal {
            position: fixed;
            top: 20px;
            left: 300px;
            width: 260px;
            background: #fff;
            border-radius: 12px;
            box-shadow: 0 8px 30px rgba(0,0,0,0.2);
            padding: 16px;
            z-index: 9999;
            display: none;
            cursor: move;
            user-select: none;
        }
        #devModal h3 {
            margin-bottom: 12px;
            font-size: 16px;
            color: #333;
        }
        #devModal button {
            width: 100%;
            margin: 4px 0;
            padding: 10px;
            border-radius: 8px;
            border: none;
            color: white;
            cursor: pointer;
        }

        @media (max-width: 768px) {
            .container {flex-direction: column;}
            .sidebar {width: 100%;height: auto;max-height: 30vh;}
            .chat-box {flex: 1;}
        }
    </style>
</head>
<body>

<div class="blur-bg" id="blurBg"></div>
<video id="bgVideo" muted loop></video>

<input type="file" id="bgInputImg" accept="image/*">
<input type="file" id="bgInputVideo" accept="video/*">
<input type="file" id="avatarInput" accept="image/*">

<div class="container">
    <div class="sidebar">
        <div class="user-info">
            <div class="avatar" id="avatar" onclick="openProfile()">
                <img id="avatarImg" src="">
            </div>
            <div>
                <div id="username" style="font-weight:bold; font-size:15px;">未登录</div>
                <div style="font-size:12px;color:#718096;">在线用户</div>
            </div>
            <button class="settings-btn" id="settingsBtn">⚙️</button>
            <div class="settings-menu" id="settingsMenu">
                <div onclick="openProfile()">👤 个人资料</div>
                <div onclick="openEditProfile()">✏️ 修改资料</div>
                <div onclick="openBgSettings()">🎨 背景设置</div>
                <div onclick="openFeedback()">💬 问题反馈</div>
                <div onclick="showAbout()">ℹ️ 关于版本</div>
                <div onclick="doLogout()" style="color:#e53e3e;">🚪 退出登录</div>
                <div onclick="openChangePwd()" style="color:#dd6b20;">🔑 修改密码</div>
            </div>
        </div>
        <button class="add-btn" id="addBtn">➕ 添加好友/创建群聊</button>
        <button class="add-btn" style="background:#dd6b20" onclick="showFriendRequests()">📩 好友申请</button>
        <div class="list" id="contactList"></div>
    </div>

    <div class="chat-box">
        <div class="chat-title">
            <div id="chatTitle">选择联系人开始聊天</div>
            <div class="chat-menu">
                <button class="menu-btn" id="menuBtn">☰</button>
                <div class="menu-popup" id="menuPopup">
                    <div onclick="blockFriend()">🚫 拉黑好友</div>
                    <div onclick="shareFriend()">🔗 分享好友</div>
                    <div onclick="deleteChat()" style="color:#e53e3e;">🗑️ 删除聊天</div>
                </div>
            </div>
        </div>
        <div class="msg-list" id="msgList"></div>
        <div class="input-box">
            <button class="file-btn" id="fileBtn">📎</button>
            <input type="file" id="fileInput" style="display: none;">
            <input type="text" id="msg-input" placeholder="输入消息...">
            <button class="send-btn" id="sendBtn">发送</button>
        </div>
    </div>
</div>

<!-- 反馈弹窗 -->
<div class="modal" id="feedbackModal">
    <span class="close-btn" onclick="closeModal('#feedbackModal')">✕</span>
    <h3>问题反馈</h3>
    <input type="text" id="feedbackContent" placeholder="请输入你的问题或建议">
    <button id="sendFeedbackBtn">提交反馈</button>
</div>

<!-- 可拖动悬浮调试面板 -->
<div id="devModal">
    <h3>🔧 调试面板</h3>
    <button onclick="clearMyData()" style="background:#e53e3e">🗑️ 清空当前用户所有信息</button>
    <button onclick="mockUser()" style="background:#4299e1">👤 生成模拟用户</button>
    <button onclick="mockChat()" style="background:#38a169">💬 生成模拟聊天</button>
    <button onclick="closeDevModal()" style="background:#718096;margin-top:10px;">❌ 关闭面板</button>
</div>

<!-- 其他弹窗 -->
<div class="modal" id="loginModal">
    <span class="close-btn" onclick="closeModal('#loginModal')">✕</span>
    <h3>用户登录</h3>
    <input type="text" id="loginUser" placeholder="请输入用户名">
    <input type="password" id="loginPwd" placeholder="请输入密码">
    <button id="loginBtn">登录</button>
    <div style="margin-top:10px;font-size:12px;">
        <span style="cursor:pointer;color:#4299e1" id="goReg">没有账号？去注册</span>
    </div>
</div>

<div class="modal" id="regModal">
    <span class="close-btn" onclick="closeModal('#regModal')">✕</span>
    <h3>用户注册</h3>
    <input type="text" id="regUser" placeholder="设置用户名">
    <input type="password" id="regPwd" placeholder="设置密码">
    <button id="regBtn">注册</button>
    <div style="margin-top:10px;font-size:12px;">
        <span style="cursor:pointer;color:#4299e1" id="goLogin">已有账号？去登录</span>
    </div>
</div>

<div class="modal" id="addModal">
    <span class="close-btn" onclick="closeModal('#addModal')">✕</span>
    <h3>添加好友 / 创建群聊</h3>
    <input type="text" id="addName" placeholder="输入名称">
    <div style="display:flex;gap:10px;">
        <button id="addFriend">添加好友</button>
        <button id="createGroup">创建群聊</button>
    </div>
</div>

<div class="modal" id="pwdModal">
    <span class="close-btn" onclick="closeModal('#pwdModal')">✕</span>
    <h3>修改密码</h3>
    <input type="password" id="oldPwd" placeholder="请输入旧密码">
    <input type="password" id="newPwd" placeholder="请输入新密码">
    <button id="savePwd">保存修改</button>
</div>

<div class="modal" id="profileModal">
    <span class="close-btn" onclick="closeModal('#profileModal')">✕</span>
    <h3>个人资料</h3>
    <div id="profileInfo" style="line-height: 1.8;"></div>
</div>

<div class="modal" id="editProfileModal">
    <span class="close-btn" onclick="closeModal('#editProfileModal')">✕</span>
    <h3>修改资料</h3>
    <div class="tip">💡 昵称每月只能修改一次</div>
    <input type="text" id="editName" placeholder="修改昵称">
    <input type="number" id="editAge" placeholder="年龄">
    <input type="text" id="editGender" placeholder="性别">
    <button onclick="document.getElementById('avatarInput').click()">更换头像</button>
    <button id="saveProfileBtn">保存</button>
    <button onclick="closeModal('#editProfileModal')" style="background:#718096;margin-left:5px;">取消</button>
</div>

<div class="modal" id="bgModal">
    <span class="close-btn" onclick="closeModal('#bgModal')">✕</span>
    <h3>背景设置</h3>
    <div style="display: flex;gap:6px;flex-wrap: wrap;margin:10px 0;">
        <button onclick="setBgColor('#f8f9fa')">默认白</button>
        <button onclick="setBgColor('#e6f7ff')">天空蓝</button>
        <button onclick="setBgColor('#fff0f6')">樱花粉</button>
        <button onclick="setBgColor('#f0fff4')">清新绿</button>
        <button onclick="setBgColor('#fff7e6')">暖黄色</button>
    </div>
    <button onclick="document.getElementById('bgInputImg').click()">上传图片背景</button>
    <button onclick="document.getElementById('bgInputVideo').click()">上传视频背景</button>
</div>

<div class="modal" id="requestModal">
    <span class="close-btn" onclick="closeModal('#requestModal')">✕</span>
    <h3>好友申请</h3>
    <div id="requestList"></div>
</div>

<script>
    let currentUser = localStorage.getItem('currentUser') || '';
    let users = JSON.parse(localStorage.getItem('users')) || [];
    let contacts = JSON.parse(localStorage.getItem('contacts')) || [];
    let messages = JSON.parse(localStorage.getItem('messages')) || {};
    let userProfiles = JSON.parse(localStorage.getItem('userProfiles')) || {};
    let friendRequests = JSON.parse(localStorage.getItem('friendRequests')) || [];
    let blockList = JSON.parse(localStorage.getItem('blockList')) || [];
    let currentTo = '', currentType = '';

    // 连续点击设置10次 → 打开可拖动悬浮调试面板
    let settingClickCount = 0;
    document.getElementById('settingsBtn').onclick = (e) => {
        e.stopPropagation();
        const menu = document.getElementById('settingsMenu');
        menu.style.display = menu.style.display === 'block' ? 'none' : 'block';
        
        settingClickCount++;
        if(settingClickCount >= 10){
            settingClickCount = 0;
            document.getElementById('devModal').style.display = 'block';
        }
    };

    // 悬浮面板拖动功能
    let isDragging = false;
    let offsetX, offsetY;
    const devModal = document.getElementById('devModal');

    devModal.addEventListener('mousedown', (e) => {
        isDragging = true;
        offsetX = e.clientX - devModal.getBoundingClientRect().left;
        offsetY = e.clientY - devModal.getBoundingClientRect().top;
        devModal.style.cursor = 'grabbing';
    });

    document.addEventListener('mousemove', (e) => {
        if (!isDragging) return;
        let x = e.clientX - offsetX;
        let y = e.clientY - offsetY;
        devModal.style.left = x + 'px';
        devModal.style.top = y + 'px';
    });

    document.addEventListener('mouseup', () => {
        isDragging = false;
        devModal.style.cursor = 'move';
    });

    // 关闭调试面板
    function closeDevModal() {
        document.getElementById('devModal').style.display = 'none';
    }

    // 聊天菜单
    document.getElementById('menuBtn').onclick = (e) => {
        e.stopPropagation();
        const p = document.getElementById('menuPopup');
        p.style.display = p.style.display === 'block' ? 'none' : 'block';
    };
    document.body.onclick = () => {
        document.getElementById('menuPopup').style.display = 'none';
        document.getElementById('settingsMenu').style.display = 'none';
    };

    // ================== 功能修复 ==================
    // 分享好友（修复）
    function shareFriend() {
        if(!currentTo) return alert('请先选择好友');
        const nick = userProfiles[currentTo]?.name || currentTo;
        const text = `好友名片：${nick}（账号：${currentTo}）`;
        navigator.clipboard.writeText(text).then(() => {
            alert('✅ 已复制好友名片：'+text);
        }).catch(()=>{
            alert('复制成功：'+text);
        });
    }

    // 拉黑好友（修复：拉黑后从列表删除）
    function blockFriend() {
        if(!currentTo || currentType !== 'friend') return alert('仅好友可拉黑');
        if(!confirm('确定拉黑该好友？拉黑后将从列表移除')) return;
        
        if(!blockList.includes(currentTo)){
            blockList.push(currentTo);
            localStorage.setItem('blockList', JSON.stringify(blockList));
        }
        
        contacts = contacts.filter(c => !(c.type === 'friend' && c.name === currentTo));
        localStorage.setItem('contacts', JSON.stringify(contacts));
        
        const key = getMsgKey();
        delete messages[key];
        localStorage.setItem('messages', JSON.stringify(messages));
        
        document.getElementById('chatTitle').innerText = '选择联系人开始聊天';
        document.getElementById('msgList').innerHTML = '';
        currentTo = ''; currentType = '';
        renderContacts();
        alert('✅ 拉黑成功，该好友已移除');
    }

    // 删除聊天
    function deleteChat() {
        if(!currentTo) return;
        if(!confirm('确定删除该聊天？记录将清空')) return;
        const key = getMsgKey();
        delete messages[key];
        localStorage.setItem('messages', JSON.stringify(messages));
        document.getElementById('msgList').innerHTML = '';
        alert('✅ 删除成功');
    }

    // ================== 反馈功能（修复报错） ==================
    function openFeedback() {
        if(!currentUser) return alert('请先登录');
        document.getElementById('feedbackModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    }

    document.getElementById('sendFeedbackBtn').onclick = () => {
        const content = document.getElementById('feedbackContent').value.trim();
        if(!content) return alert('请输入反馈内容');
        try {
            const user = currentUser || '未登录用户';
            const subject = `【聊天系统反馈】来自用户：${user}`;
            const body = `反馈用户：${user}\n反馈内容：${content}`;
            const mail = `mailto:qw123584688@163.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(body)}`;
            window.open(mail, '_blank');
            alert('✅ 反馈已提交，将发送到客服邮箱');
        } catch (e) {
            alert('反馈已收到：' + content);
        }
        closeModal('#feedbackModal');
        document.getElementById('feedbackContent').value = '';
    };

    // ================== 调试功能 ==================
    function clearMyData() {
        if(!currentUser) return alert('请先登录');
        if(!confirm('确定清空当前用户的所有资料、好友、聊天记录？')) return;
        
        contacts = contacts.filter(c => !(c.type === 'friend' && c.name === currentUser));
        messages = {};
        friendRequests = friendRequests.filter(r => r.from !== currentUser && r.to !== currentUser);
        blockList = [];
        
        localStorage.setItem('contacts', JSON.stringify(contacts));
        localStorage.setItem('messages', JSON.stringify(messages));
        localStorage.setItem('friendRequests', JSON.stringify(friendRequests));
        localStorage.setItem('blockList', JSON.stringify(blockList));
        
        renderContacts();
        document.getElementById('msgList').innerHTML = '';
        document.getElementById('chatTitle').innerText = '选择联系人开始聊天';
        currentTo = ''; currentType = '';
        alert('✅ 当前用户信息已全部清空');
    }

    function mockUser() {
        if(users.length === 0) {
            users = [{user:'test1',pwd:'123'},{user:'test2',pwd:'123'}];
            localStorage.setItem('users', JSON.stringify(users));
        }
        alert('✅ 已生成测试用户：test1 / test2 密码：123');
    }

    function mockChat() {
        if(!currentUser) return alert('请先登录');
        const mockName = '测试助手';
        const key = 'friend_测试助手';
        messages[key] = [
            {user:'测试助手',text:'你好呀！',time:new Date().toLocaleString(),type:'text'},
            {user:currentUser,text:'你好！',time:new Date().toLocaleString(),type:'text'},
            {user:'测试助手',text:'这是模拟聊天消息',time:new Date().toLocaleString(),type:'text'}
        ];
        if(!contacts.some(c=>c.name==='测试助手')){
            contacts.push({type:'friend',name:'测试助手'});
        }
        userProfiles['测试助手'] = {name:'测试助手',avatar:'',age:'20',gender:'机器人'};
        localStorage.setItem('messages', JSON.stringify(messages));
        localStorage.setItem('contacts', JSON.stringify(contacts));
        localStorage.setItem('userProfiles', JSON.stringify(userProfiles));
        renderContacts();
        alert('✅ 已生成模拟聊天');
    }

    // ================== 原有功能 ==================
    function setBgColor(color) {
        document.body.style.background = color;
        document.body.style.backgroundImage = 'none';
        document.getElementById('bgVideo').style.display = 'none';
        closeModal('#bgModal');
    }

    document.getElementById('bgInputImg').onchange = e => {
        const file = e.target.files[0];
        if(!file) return;
        const url = URL.createObjectURL(file);
        document.body.style.backgroundImage = `url(${url})`;
        document.body.style.backgroundSize = 'cover';
        document.getElementById('bgVideo').style.display = 'none';
    };

    document.getElementById('bgInputVideo').onchange = e => {
        const file = e.target.files[0];
        if(!file) return;
        const url = URL.createObjectURL(file);
        const video = document.getElementById('bgVideo');
        video.src = url;
        video.style.display = 'block';
        video.play();
        document.body.style.backgroundImage = 'none';
    };

    window.onload = () => {
        if (!currentUser) {
            document.getElementById('loginModal').style.display = 'block';
            document.getElementById('blurBg').style.display = 'block';
        } else {
            loadProfile();
            document.getElementById('blurBg').style.display = 'none';
        }
        renderContacts();
        document.getElementById('avatarInput').onchange = e => {
            const file = e.target.files[0];
            if(!file) return;
            const url = URL.createObjectURL(file);
            document.getElementById('avatarImg').src = url;
            if(currentUser) userProfiles[currentUser].avatar = url;
            localStorage.setItem('userProfiles', JSON.stringify(userProfiles));
            renderContacts();
        };
    };

    function closeModal(id) {
        document.querySelectorAll('.modal').forEach(m => m.style.display = 'none');
        document.getElementById('blurBg').style.display = 'none';
    }

    function loadProfile() {
        if(!userProfiles[currentUser]) {
            userProfiles[currentUser] = {name:currentUser, avatar:'', age:'', gender:'', lastRename:0};
        }
        const p = userProfiles[currentUser];
        document.getElementById('username').innerText = p.name;
        document.getElementById('avatarImg').src = p.avatar || '';
        localStorage.setItem('userProfiles', JSON.stringify(userProfiles));
    }

    function openProfile(targetUser = null) {
        if(!currentUser) return;
        const user = targetUser || currentUser;
        const p = userProfiles[user] || {name:user, avatar:'', age:'未设置', gender:'未设置'};
        document.getElementById('profileInfo').innerHTML = `
            昵称：${p.name}<br>
            年龄：${p.age || '未设置'}<br>
            性别：${p.gender || '未设置'}
        `;
        document.getElementById('profileModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    }

    function openEditProfile() {
        if(!currentUser) return;
        const p = userProfiles[currentUser];
        document.getElementById('editName').value = p.name;
        document.getElementById('editAge').value = p.age || '';
        document.getElementById('editGender').value = p.gender || '';
        document.getElementById('editProfileModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    }

    document.getElementById('saveProfileBtn').onclick = () => {
        if(!currentUser) return;
        const p = userProfiles[currentUser];
        const now = Date.now();
        const oneMonth = 30*24*60*60*1000;
        
        if(document.getElementById('editName').value !== p.name) {
            if(now - p.lastRename < oneMonth) {
                alert('每月只能修改一次昵称！');
                return;
            }
            p.lastRename = now;
        }
        
        p.name = document.getElementById('editName').value;
        p.age = document.getElementById('editAge').value;
        p.gender = document.getElementById('editGender').value;
        
        localStorage.setItem('userProfiles', JSON.stringify(userProfiles));
        loadProfile();
        renderContacts();
        closeModal('#editProfileModal');
        alert('保存成功！');
    };

    function openBgSettings() {
        document.getElementById('bgModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    }

    function showAbout() {
        alert('智能聊天系统\n版本：悬浮调试版\n✅ 可拖动悬浮调试面板');
    }

    document.getElementById('goReg').onclick = () => {
        document.getElementById('loginModal').style.display = 'none';
        document.getElementById('regModal').style.display = 'block';
    };
    document.getElementById('goLogin').onclick = () => {
        document.getElementById('regModal').style.display = 'none';
        document.getElementById('loginModal').style.display = 'block';
    };

    document.getElementById('regBtn').onclick = () => {
        const user = document.getElementById('regUser').value.trim();
        const pwd = document.getElementById('regPwd').value.trim();
        if (!user || !pwd) return alert('请输入用户名和密码');
        const hasUser = users.some(item => item.user === user);
        if (hasUser) return alert('用户名已存在');
        users.push({ user, pwd });
        localStorage.setItem('users', JSON.stringify(users));
        alert('注册成功！请登录');
        document.getElementById('regModal').style.display = 'none';
        document.getElementById('loginModal').style.display = 'block';
    };

    document.getElementById('loginBtn').onclick = () => {
        const user = document.getElementById('loginUser').value.trim();
        const pwd = document.getElementById('loginPwd').value.trim();
        if (!user || !pwd) return alert('请输入用户名和密码');
        const target = users.find(item => item.user === user && item.pwd === pwd);
        if (!target) return alert('用户名或密码错误');
        currentUser = user;
        localStorage.setItem('currentUser', user);
        loadProfile();
        document.getElementById('loginModal').style.display = 'none';
        document.getElementById('blurBg').style.display = 'none';
        renderContacts();
    };

    function doLogout() {
        if(!currentUser) return alert("未登录！");
        currentUser = ''; 
        localStorage.removeItem('currentUser');
        document.getElementById('username').innerText = '未登录';
        document.getElementById('chatTitle').innerText = '选择联系人开始聊天';
        document.getElementById('msgList').innerHTML = '';
        currentTo = ''; currentType = '';
        alert('退出登录成功');
        document.getElementById('loginModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    }

    function openChangePwd() {
        if(!currentUser) return alert("请先登录！");
        document.getElementById('pwdModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    }
    document.getElementById('savePwd').onclick = () => {
        const old = document.getElementById('oldPwd').value.trim();
        const newPwd = document.getElementById('newPwd').value.trim();
        if(!old || !newPwd) return alert("请填写完整");
        const index = users.findIndex(item=>item.user === currentUser && item.pwd === old);
        if(index === -1) return alert("旧密码错误");
        users[index].pwd = newPwd;
        localStorage.setItem('users',JSON.stringify(users));
        alert("修改成功！");
        closeModal('#pwdModal');
        document.getElementById('oldPwd').value = '';
        document.getElementById('newPwd').value = '';
    };

    function showFriendRequests() {
        if(!currentUser) return;
        const list = document.getElementById('requestList');
        list.innerHTML = '';
        const myReqs = friendRequests.filter(r => r.to === currentUser);
        if(myReqs.length === 0) {
            list.innerHTML = '<div style="text-align:center; padding:20px;">暂无好友申请</div>';
        } else {
            myReqs.forEach((req, idx) => {
                const item = document.createElement('div');
                item.className = 'request-item';
                item.innerHTML = `
                    <span>${req.from}</span>
                    <div>
                        <button class="request-btn agree" onclick="agreeRequest(${idx})">同意</button>
                        <button class="request-btn refuse" onclick="refuseRequest(${idx})">拒绝</button>
                    </div>
                `;
                list.appendChild(item);
            });
        }
        document.getElementById('requestModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    }

    function agreeRequest(idx) {
        const req = friendRequests[idx];
        contacts.push({type:'friend', name:req.from});
        contacts.push({type:'friend', name:req.to});
        friendRequests.splice(idx, 1);
        saveAll();
        showFriendRequests();
        renderContacts();
        alert('已添加好友！');
    }

    function refuseRequest(idx) {
        friendRequests.splice(idx, 1);
        saveAll();
        showFriendRequests();
        alert('已拒绝');
    }

    document.getElementById('addBtn').onclick = () => {
        if(!currentUser) return alert("请先登录！");
        document.getElementById('addModal').style.display = 'block';
        document.getElementById('blurBg').style.display = 'block';
    };

    document.getElementById('addFriend').onclick = () => {
        const name = document.getElementById('addName').value.trim();
        if (!name) return;
        if(name === currentUser) return alert('不能添加自己');
        const userExist = users.some(u => u.user === name);
        if(!userExist) return alert('该用户不存在');
        const isFriend = contacts.some(c => c.type === 'friend' && c.name === name);
        if(isFriend) return alert('已是好友');
        const isReq = friendRequests.some(r => r.from === currentUser && r.to === name);
        if(isReq) return alert('已发送申请');
        
        friendRequests.push({from:currentUser, to:name});
        localStorage.setItem('friendRequests', JSON.stringify(friendRequests));
        closeModal('#addModal');
        alert('好友申请已发送！等待对方同意');
    };

    document.getElementById('createGroup').onclick = () => {
        const name = document.getElementById('addName').value.trim();
        if (!name) return;
        const exist = contacts.some(i=>i.type==='group'&&i.name===name);
        if(exist) return alert("该群聊已存在");
        contacts.push({type: 'group', name});
        saveContacts(); renderContacts(); closeModal('#addModal');
    };

    function renderContacts() {
        const list = document.getElementById('contactList');
        list.innerHTML = '';
        const others = contacts.filter(c => !(c.type === 'friend' && c.name === currentUser));
        
        others.forEach(item => {
            if(item.type === 'friend' && blockList.includes(item.name)) return;
            const div = document.createElement('div');
            div.className = 'item';
            const avatar = userProfiles[item.name]?.avatar || '';
            const showName = userProfiles[item.name]?.name || item.name;
            div.innerHTML = `
                <div class="msg-avatar"><img src="${avatar}" onclick="openProfile('${item.name}')"></div>
                <span>${item.type === 'group' ? '👥' : '👤'} ${showName}</span>
            `;
            div.onclick = () => {
                currentTo = item.name; currentType = item.type;
                document.getElementById('chatTitle').innerText = userProfiles[currentTo]?.name || currentTo;
                renderMsg();
            };
            list.appendChild(div);
        });
    }

    function getMsgKey(){ return currentType + "_" + currentTo; }

    // 发送消息（修复：可发数字）
    document.getElementById('sendBtn').onclick = sendMsg;
    document.getElementById('msg-input').onkeydown = e => e.key === 'Enter' && sendMsg();
    function sendMsg() {
        const text = document.getElementById('msg-input').value.trim();
        if (!text || !currentTo || !currentUser) return;
        if(blockList.includes(currentTo)) return alert('已拉黑该好友');
        
        const msg = {user: currentUser, text, time: new Date().toLocaleString(), type:'text'};
        const key = getMsgKey();
        if (!messages[key]) messages[key] = [];
        messages[key].push(msg);
        saveMsg(); renderMsg();
        document.getElementById('msg-input').value = '';
    }

    document.getElementById('fileBtn').onclick = () => document.getElementById('fileInput').click();
    document.getElementById('fileInput').onchange = e => {
        const file = e.target.files[0];
        if (!file || !currentTo) return;
        const url = URL.createObjectURL(file);
        const msg = {user: currentUser, text:`📎 ${file.name}`, time:new Date().toLocaleString(), type:'file', url};
        const key = getMsgKey();
        if (!messages[key]) messages[key] = [];
        messages[key].push(msg);
        saveMsg(); renderMsg();
    };

    function renderMsg() {
        const list = document.getElementById('msgList');
        list.innerHTML = '';
        const key = getMsgKey();
        if (!messages[key]) return;
        messages[key].forEach(msg => {
            const row = document.createElement('div');
            const isMe = msg.user === currentUser;
            row.className = `msg-row ${isMe ? 'me' : ''}`;
            
            const avatar = document.createElement('div');
            avatar.className = 'msg-avatar';
            const img = userProfiles[msg.user]?.avatar || '';
            avatar.innerHTML = `<img src="${img}" onclick="openProfile('${msg.user}')">`;
            
            const content = document.createElement('div');
            content.className = `msg ${isMe ? 'my-msg' : 'other-msg'} ${msg.type==='file'?'file-msg':''}`;
            
            if(msg.type === 'file'){
                content.innerHTML = `${msg.text}<br><small>${msg.time}</small>`;
                content.onclick = () => {
                    const a = document.createElement('a');
                    a.href=msg.url; a.download=''; a.target='_blank'; a.click();
                };
            }else{
                content.innerText = `${msg.text}\n${msg.time}`;
            }
            
            row.appendChild(avatar);
            row.appendChild(content);
            list.appendChild(row);
        });
        list.scrollTop = list.scrollHeight;
    }

    function saveContacts() {localStorage.setItem('contacts', JSON.stringify(contacts));}
    function saveMsg() {localStorage.setItem('messages', JSON.stringify(messages));}
    function saveAll() {
        saveContacts(); saveMsg();
        localStorage.setItem('friendRequests', JSON.stringify(friendRequests));
    }
</script>
</body>
</html>
