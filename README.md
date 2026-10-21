# Embedded Plays · 嵌入式软件开发互动课程

把 147 章嵌入式学习教程重排为 **6 卷课程馆 + 10 个基础深读页**，每页都是可离线打开的独立 HTML：讲义、动画、互动实验、学习路线与复盘自测。

**在线学习：** <https://meimei5211314.github.io/Embedded-Plays/>

## 开始学习

打开 [index.html](index.html)（或直接访问上面的在线地址）。

推荐学习闭环：

1. **读讲义 + 做实验**：正文、互动实验室、学习路线。
2. **自评 + 留卡点笔记**：能讲清 / 有点卡 / 没懂，三档自评；选「能讲清」自动标记已读。
3. **进复盘队列**：闭卷回忆、面试追问、故障排查表；笔记与书签可导出 Markdown。

学习进度、自评、笔记和书签保存在浏览器 localStorage，不上传服务器。

## 内容结构

| 页面 | 内容 |
| --- | --- |
| [index.html](index.html) | 总目录：六卷导航、147 章检索、进度与继续学习 |
| [vol1-toolchain-mcu.html](vol1-toolchain-mcu.html) | 工具链与 Cortex-M |
| [vol2-soc-rtos.html](vol2-soc-rtos.html) | SoC 与 RTOS |
| [vol3-linux-android.html](vol3-linux-android.html) | Linux 与 Android |
| [vol4-bus-product.html](vol4-bus-product.html) | 总线与产品化 |
| [vol5-algorithms-performance.html](vol5-algorithms-performance.html) | 算法与性能 |
| [vol6-heterogeneous-expert.html](vol6-heterogeneous-expert.html) | 异构与专家 |
| [course-hub.html](course-hub.html) | 总目录别名页，保留给卷内返回链接 |
| `ch1` – `ch9a` 深读页 | 语言、内存、调试、链接布局、数据结构、架构、质量与 AI 协作 |

### 深链

- `?view=read|lab|path|review`：直达讲义 / 实验室 / 学习路线 / 复盘
- `?lab=N`：直达第 N 个实验
- `?sec=<anchor>`：直达某个知识小节

## 本地运行

直接双击 `index.html` 即可。若浏览器限制本地文件的部分能力，可启动静态服务器：

```bash
python -m http.server 8000
```

然后访问 <http://localhost:8000/>。

## 部署

仓库根目录即站点目录，GitHub Pages 从 `main` 分支根路径构建；每次推送自动更新。`.nojekyll` 用于关闭 Jekyll 处理，确保 HTML 原样发布。

## 来源与说明

内容基于开源嵌入式学习教程 <https://zn-phd336699.github.io/Embedded-Learning/> 重构；讲义中的实验与项目描述用于教学演示。
