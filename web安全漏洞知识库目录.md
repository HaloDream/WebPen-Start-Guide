Web安全漏洞知识库目录
===

A. 客户端安全漏洞
攻击主要发生在用户浏览器或需要用户交互的场景。

A1. 跨站脚本

A1.1 反射型XSS - PortSwigger Academy, DVWA, WebGoat

A1.2 存储型XSS - PortSwigger Academy, DVWA, bWAPP

A1.3 基于DOM的XSS - PortSwigger Academy, Google XSS Game

A2. 跨站请求伪造

A2.1 传统型CSRF - DVWA, WebGoat, bWAPP

A2.2 JSON/API型CSRF - PortSwigger Academy

A3. 点击劫持与UI伪装

A3.1 点击劫持 - 实验环境需自建

A3.2 拖拽劫持与文本注入 - 实验环境需自建

A4. 客户端资源操控

A4.1 Web存储（Local/SessionStorage）不安全 - 通常结合XSS演示

A4.2 跨源资源共享配置错误 - PortSwigger Academy

A4.3 PostMessage通信滥用 - PortSwigger Academy

B. 服务端注入与解释器漏洞
核心特征：不可信数据被解释器当作代码或命令执行。

B1. 数据库查询注入

B1.1 SQL注入 - DVWA, WebGoat, PortSwigger Academy

B1.2 NoSQL注入 - OWASP Juice Shop, 自建环境

B2. 操作系统命令注入

B2.1 经典命令注入 - DVWA, WebGoat, PentesterLab

B2.2 参数注入 - 实验环境需自建

B3. 代码与模板注入

B3.1 服务器端模板注入 - PortSwigger Academy, SSTI Labs

B3.2 表达式语言注入 - WebGoat (部分), 自建环境

B3.3 动态代码执行 - 自建环境

B4. 协议与目录服务注入

B4.1 LDAP注入 - WebGoat, bWAPP

B4.2 XPath注入 - WebGoat, bWAPP

B4.3 邮件命令注入 - 通常见于CTF题目

C. 服务端文件与资源处理漏洞
核心特征：对用户提交的文件、路径或资源标识符处理不当。

C1. 文件上传漏洞

C1.1 不受限制的文件上传 - DVWA, Upload-Labs, bWAPP

C1.2 文件类型/内容验证绕过 - Upload-Labs, PentesterLab

C2. 路径遍历与文件包含

C2.1 路径遍历 - DVWA, WebGoat, Path Traversal Labs

C2.2 本地/远程文件包含 - DVWA, bWAPP (RFI)

C3. XML外部实体攻击

C3.1 经典XXE（文件读取） - PortSwigger Academy, WebGoat, bWAPP

C3.2 XXE盲注与SSRF - PortSwigger Academy

C4. 服务器端请求伪造

C4.1 基础SSRF（访问内部服务） - PortSwigger Academy, SSRF Labs

C4.2 盲SSRF与高级利用 - PortSwigger Academy

D. 身份、会话与访问控制漏洞
核心特征：系统无法正确识别用户或控制其对资源的访问。

D1. 身份认证缺陷

D1.1 弱口令与暴力破解 - DVWA, bWAPP, WebGoat

D1.2 密码重置逻辑缺陷 - WebGoat, PortSwigger Academy

D1.3 多因素认证绕过 - 自建实验环境

D1.4 JSON Web令牌实现缺陷 - PortSwigger Academy JWT Labs

D2. 会话管理缺陷

D2.1 会话固定 - DVWA, WebGoat, bWAPP

D2.2 会话令牌泄露与预测 - DVWA, WebGoat

D3. 授权与访问控制缺陷

D3.1 水平越权 - PortSwigger Academy, OWASP Juice Shop

D3.2 垂直越权 - DVWA, WebGoat, bWAPP

D3.3 不安全的直接对象引用 - WebGoat, OWASP Juice Shop

E. 应用逻辑与配置漏洞
核心特征：业务流程、状态机或系统配置存在缺陷。

E1. 业务逻辑缺陷

E1.1 竞争条件 - 自建实验环境， Race Condition Lab

E1.2 流程/状态机绕过 - OWASP Juice Shop

E1.3 数据/金额篡改 - OWASP Juice Shop, WebGoat

E2. 安全配置错误

E2.1 默认凭证与调试接口 - Metasploitable, VulnHub

E2.2 不安全的HTTP方法 - bWAPP, DVWA

E2.3 目录列表与信息泄露 - DVWA, bWAPP

E2.4 安全响应头缺失 - 自建环境或SecurityHeaders.io扫描

E3. 数据处理缺陷

E3.1 批量分配 - OWASP Juice Shop, WebGoat

E3.2 不安全的反序列化 - PortSwigger Academy, WebGoat

E3.3 正则表达式拒绝服务 - 自建环境

F. 通信、协议与架构层漏洞
核心特征：网络协议处理、系统架构或组件交互层面的问题。

F1. 传输层与协议漏洞

F1.1 明文传输与弱TLS配置 - 扫描工具演示 (如 testssl.sh)

F1.2 HTTP请求走私 - PortSwigger Academy HTTP Request Smuggling Labs

F1.3 HTTP参数污染 - WebGoat, bWAPP

F1.4 WebSocket安全漏洞 - 自建实验环境

F2. 第三方组件与供应链漏洞

F2.1 已知框架/库漏洞利用 - VulnHub (如 Struts2, ThinkPHP)

F2.2 依赖链混淆攻击 - 概念演示， 较新领域

F3. API与新兴架构漏洞

F3.1 API未授权/过度数据暴露 - OWASP Juice Shop API Challenges

F3.2 GraphQL安全 - 自建实验环境

F3.3 云/容器配置错误 - CloudGoat, Flaws.cloud