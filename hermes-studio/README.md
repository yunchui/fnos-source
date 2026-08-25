<p>🐴面向 Hermes Agent 的本地运行时和 Web 控制台。Agent 对话、可视化工作流、模型与 Profile 管理、网页浏览、Coding Agent 和本地运行环境都在一个界面中完成。</p>
<p><strong>部署说明：</strong>本包以官方预构建产物 + bundled node_modules 方式安装（非 Docker），已将 hermes-web-ui 的 node_modules 与 Hermes Agent 的 browser tools + TUI 依赖（hermes-agent-node）一并预装进 FPK，首次安装自动使用飞牛 Node.js v24 运行时并把预装依赖复制到数据目录，后台安装不再联网跑 npm install。启动后默认监听 8648 端口，通过应用图标即可在浏览器打开 Web UI。</p>
<p><strong>核心能力：</strong><br/>
• Agent 聊天：Socket.IO 流式运行 Hermes Agent<br/>
• 本地控制台：管理 profiles、providers、models、凭证、记忆、技能、插件、日志<br/>
• 自动化：平台渠道、cron 定时任务、看板任务、群聊房间、MCP 服务器<br/>
• 工作区工具：文件浏览器、Web 终端、语音输入/输出、编码 Agent、设备发现<br/>
</p>
<p><strong>来源：</strong>本包由 <a href="https://github.com/yunchui/Fnos-Hermes-Studio">yunchui/Fnos-Hermes-Studio</a> 自动构建，上游为 <a href="https://github.com/EKKOLearnAI/hermes-studio">EKKOLearnAI/hermes-studio</a>。</p>
