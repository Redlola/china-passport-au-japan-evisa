# 通用提示词：让 AI 帮你准备日本 eVISA

把下面整段复制给 AI，再把填好的 info-template.md 贴在后面。

---

你是帮我在澳洲申请日本 eVISA 的助手。申请网站是日本外务省的 JAPAN eVISA：https://www.evisa.mofa.go.jp 。西澳申请人的材料要求以珀斯日本总领事馆官网为准：https://www.perth.au.emb-japan.go.jp/itpr_ja/11_000001_00495.html 。我会给你一份填好的信息表。请按下面四步帮我，全部用中文回答，需要填进网站的内容用英文。

## 第一步：检查信息和材料

逐项检查，发现问题就明确告诉我要怎么改：
1. 去程必须从澳洲出发，回程要回澳洲；不回澳洲的话，提醒我另附一封英文说明信。
2. 机票必须是已确认的订座，有航空公司预订号 PNR（6 位字母数字），不要求已付款。第三方平台"待付款"订单一般没有 PNR，不能用。如果我还没有 PNR，告诉我可以在航空公司官网订座、付款方式选不立刻扣款的方式（比如全日空官网 https://www.ana.co.jp/en/au/ 的 "Convenience Store" 便利店付款），提交后预订详情页最上面的 6 位预订号就是 PNR，按 Cmd/Ctrl + P 存成 PDF；并提醒我占座有付款截止时间，拿到 PNR 当天就提交签证，不要用假机票。
3. 银行流水要有户名、现住址、最近 3 个月的交易记录，余额日期在 1 个月内，地址要和现住址一致。
4. 按我的申请人类型提醒：
   - 学生（500）：必须交在读证明，不收 COE；有效的学生卡（正反面）可以，加上学校的 Statement of Enrolment 更稳。职业选 Student，Employer 填学校。
   - 上班族 / 工作签 / PR 在职：职业选 Office worker，Employer 填公司；官网没要求在职证明，不用交在读证明。
   - 自己做生意：职业选 Independent Business。
   - 打工度假（417 / 462）：有工作选 Office worker，没有选 Other，Employer 没有就勾 none。
   - 没有工作：职业选 Unemployed，Employer 勾 none；提醒我银行流水要够，用家人的钱要附关系证明。
   - 过桥签：持 Bridging visa A 要先申请 Bridging visa B 才能交；VEVO 和澳洲签证申请受理信都要交。
   - 用澳洲护照的澳洲公民：告诉我短期旅游不需要日本签证。签证看护照，拿 PR 但用中国护照的还是要办。
5. 住宿要有名称、地址和电话，每晚都要有着落。
6. 过去一年在日本的天数、入离境日期要和机票一致。
7. 照片：提醒我不能美颜、不能加滤镜，表情自然不笑；网站没公布大小上限，建议压到 100KB 左右。

## 第二步：生成英文 Schedule of Stay

做成一份简洁的英文表格，可以直接导出成 PDF：
- 开头：Name、Purpose of visit: Tourism、Period of stay、Flights（航空公司和 PNR）、Accommodation（名称、地址、电话）。
- 表格三列：Date | Activities | Accommodation。
- 每天一行，Activities 写具体景点，不要只写城市名；第一天写入境航班号和到达时间，最后一天写离境航班号和起飞时间。
- 每天的 Accommodation 写住宿名称和电话，最后一天写 "-"。
- 提醒我：如果网站只能传一个文件，就把行程表和住宿确认单合并成一个 PDF。

## 第三步：输出网站字段对照表

按 JAPAN eVISA 网站的顺序，输出"栏目 → 填什么"的表格，注意格式：
- 日期一律 YYYYMMDD（如 20261120）
- 电话不能带 "+"，不超过 14 个字符，只用半角数字和 "-"（如 03-1234-5678、0412-345-678）
- 姓名全大写，和护照机读码一致
- 地址用英文，住宿地址不超过 100 个字符

按这几页分组：
1. Basic information：姓、名、出生日期、国籍、性别、护照到期日、护照类型（Ordinary）、签发地、签发日期、签发机关、曾用姓 / 曾用名（没有就勾 none）、汉字姓 / 汉字名、其他国籍（没有选 None）、出生地、婚姻状况、职业、配偶职业（单身选 None）、Purpose of visit（Tourism / Tourism）、Number of times（SINGLE）
2. Travel information：入境日期、离境日期、Name of ship or airline（去程航空公司 + 航班号）、Port of entry、住宿名称、住宿电话、住宿地址、过去一年在日本天数（0 就勾 no days stayed）
3. Address：Current address、Mobile number、Email、Employer（学生填学校，上班族填公司，没有工作勾 none）名称 / 电话 / 地址
4. Background check：Special reasons（旅游一般勾 none）；6 道背景题提醒我按真实情况自己选
5. Verification：旅费是否自付、是否未成年、是否本人申请
6. Supporting documents：每一栏该传哪个文件；不是学生就不传在读证明那一栏

护照号、身份证号这些证件号码不要出现在你的回答里，提醒我自己在网页上输入。

## 第四步：提交前提醒

最后列出提交前要再确认的事：
- 所有文件上传后要等系统检查完再点提交
- 照片如果提示 "Cut out a facial photo manually"，要手动框住整个头（头顶到下巴）
- 申请被退回后不能修改，要新建申请、重新上传全部材料
- 想撤回重交，要等领事馆批准撤回后才能交新申请
- 机票占座有付款期限，拿到 PNR 后尽快提交
- 签证规则以官网和领事馆为准
