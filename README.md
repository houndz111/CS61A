# CS61A — Structure and Interpretation of Computer Programs

My solutions and progress for [UC Berkeley CS61A](https://cs61a.org/). Personal study log, not an official repository.

---

## 关于这个仓库

这是学习 CS61A 的作业记录。仓库只保存源码和题目配置，**不包含 `ok` 判题器与本地编辑器**（见下方「怎么跑」一节）。

## 进度

| 模块                          | 内容                                      | 状态                        |
| ----------------------------- | ----------------------------------------- | --------------------------- |
| HW 01                         | Functions, Control                        | 已完成 6/6                  |
| HW 02                         | Higher-Order Functions                    | 已完成                      |
| HW 03–06                      | Recursion, Lists, Trees, OOP              | 未开始                      |
| Lab 00                        | Setup                                     | 已完成                      |
| Lab 01                        | Functions, Control                        | 已完成                      |
| Lab 02–10                     | HOF, Lists, Iterators, OOP, Trees, Scheme | 未开始                      |
| Project: Hog                  | The Game of Hog                           | Q1–Q5 已完成，Q6–Q13 未开始 |
| Project: Cats / Ants / Scheme | —                                         | 未开始                      |

## 目录结构

```
HW/         家庭作业 hw01–hw10（.py / .scm / .sql）
Lab/        实验 lab00–lab12
Project/    hog、cats、ants、scheme 四个项目
```

每个作业目录里：`*.py`（或 `.scm` / `.sql`）是要填的文件，`tests/` 是测试用例，`*.ok` 是判题配置。

## 怎么跑

Windows 上用 `py` 代替 `python3`：

```bash
cd Project/hog

py ok -q 01 --local        # 判某一题（题号不带括号）
py ok --local              # 判整个文件
py ok -u -q 06 --local     # 先解锁再判（部分题目需要）
```

第一次运行会问是否向 61A-bot 发送统计，输 `never` 即可。

**注意：clone 本仓库后 `ok` 是缺失的。** 因为 `ok` 判题器有 27 份、每份约 2.8MB，`editor/` 本地编辑器每份近 10MB，全部提交会让仓库膨胀到 150MB 以上，所以我在 `.gitignore` 里排除了它们。需要判题时，把课程原始作业包里的 `ok` 拷进对应目录即可，其余文件都是完整的。

## 一点说明

- 课程材料（题面、测试、骨架代码）版权归 UC Berkeley CS61A 教学团队所有，这里仅作个人学习记录。
