This is a demo vault for [KG Notes](https://forum-zh.obsidian.md/t/topic/2059) (Knowledge Graph Notes). This vault will explain the creation and basic use of KG Notes. To experience the full feature, you need to use this vault with the [path-finder](https://github.com/jerrywcy/obsidian-path-finder) plugin (which is installed in this vault).

(sorry for my poor English. If you know Chinese, you can read [Chinese Version](https://github.com/11-check-it-out/KGnotes-demo).)

# I. Introduction

## 1. The origin: what do we really need?

I'm sure many of you, are wondering how to use note taking software, or what the notes can give us.

This question has been bothering me ever since taking notes. I had pinned my hopes on note-taking software, hoping that it would tell me the answer. So over the past few years, I have switched to different note-taking software — Evernote, OneNote, Notion, RoamResearch, Obsidian. Every software has told me that I should build my own second brain, that I should generate new insights from my notes. But how to do this? The softwares didn't tell me the answer.

Thus, I saw this as a methodological problem and turned my attention to various note-taking methods. I hoped that these methods would turn my note-taking software into my second brain and allow me to generate new inspiration from my notes. From the original Luhmann Note Box, to the Zettlekasten, to the later series of methods based on them, I have used each of these methods one by one. More than the note taking software itself, these methods are really teaching me how to organise my notes and how to get new ideas out of them. But I still found it a little bit confusing because these methods were more focused on delivering ideas without giving rigorous steps that could be taken to build a personal system of notes -- they were more about telling me the reason and the vision for doing so. When I tried to understand how to build my own system of knowledge, I was always told: "Everyone's system of knowledge is different, you can't copy me, you have to learn from my ideas and build your own system". However, after six months of studying, I couldn't figure it out. So I started to look for a more rigorous approach.

In a roundabout way, in 2020, I came across cognitive psychology, library science and information organisation. Since then, I have been looking at the issue from a more professional perspective, building on the findings of previous research.

After reading a series of specialist books, I finally understood the essence of the purpose of note taking, which is to organise personal knowledge so that it can be quickly retrieved when needed. As knowledge workers, we always need knowledge to help us solve problems -- this includes both using existing knowledge to solve procedural problems, such as recalling known steps to complete a procedure, and using existing knowledge to infer solutions to non-procedural problems, such as researching a new marketing plan, writing a paper about a new problem. In this process, it is crucial to be able to quickly recall existing knowledge. This can be implemented either by enhancing the memory of existing knowledge (e.g. with memory software such as SuperMemo or Anki) or by using external media to record existing knowledge and retrieve it quickly when needed. The latter is the fundamental purpose of "building a second brain" and the reason why people take notes for classes, papers and work.

## 2. Methods for efficient searching

How can we efficiently retrieve existing knowledge? Many people's first thought is to use a full-text search. It is true that this method is efficient, but not always - full-text search does not solve the problem of multiple words with one meaning. For example, when we search for "potato" in full text, the software automatically filters for content containing the word "Spud". So, we need to use other methods to solve this problem.

Essentially, the process of retrieving information is the process of obtaining relevant information through retrieval symbols. For example, when we use a search engine or full-text search, the keywords we use are the retrieval symbols used to obtain the relevant information. The design of the retrieval symbols has a direct impact on the efficiency of our search. For example, what do we intuitively do when we need to find potato-related content immediately? Our first thought must be to look for notes tagged with potatoes, or for those in the crops/potatoes folder, but never to think that I made notes about potatoes someday (in this case timestamps are a bad choice). Thus, retrieval symbols must be designed around semantic and informational subjects. Librarians identified this problem early and invented classification method and subject heading method to address it.

## 3. Towards automatic deduction

Based on the classification and subject heading method invented by librarians, we can truly implement a personalised note system that allows efficient retrieval of existing knowledge. This note-taking system is like having a well-organised fridge for cooking, from which we can quickly find the ingredients we need.

But so far, this note system is only working as a repository of material. Can we make this note system a little smarter to automatically explore the potential insights hidden in the material?

This brings us to the application of knowledge graphs. Based on knowledge graphs, we can easily discover potential connections between entities. For example, if B is known to be a friend of A, D is a friend of B and E is a friend of D, we can deduce that A and D may also know each other. Could we not apply this logic to our note taking system?

![Pasted image 20221006142436](Attachments/Pasted%20image%2020221006142436.png)

I studied further the content related to knowledge graphs. As a result, I found that if I wanted to implement the above deductions, first of all the knowledge had to be represented symbolically. And this coincides with the subject heading method which was described in the previous section. Thus, the KG notes method, based on the idea of a subject heading method and knowledge graph, was born. 

# Ⅱ. KG Notes Method

Now I will briefly introduce KG notes method. (If you want more details, you can try reading [the Chinese version of the instructions](https://forum-zh.obsidian.md/t/topic/2059).)

## 1. Concept introduction

In the KG notes method, all information can be divided into three categories: 

1) a comprehensive discussion of a concept or entity;
2) a discussion of an aspect of a concept or entity;
3) a discussion of the relationship of a concept or entity to other concepts or entities.

And according to knowledge graph, we have three types of notes:

1) Concept notes, which are used to record information about a concept. For example, potato-related content is recorded in the note *Potato*.
2) Entity notes, which are used to record information about an entity. For example, Amazon.com related content is recorded in the note *Amazon.com*.
3) Relationship notes,  which are used to record information about a relationship. For example, notes about the difference between potatoes and sweet potatoes are recorded in the note *Potato - compare - (sweet potato)*.

All notes reveal their content through their titles. It is important to note that there are four types of titles for relationship notes, depending on the subject heading method:

- Relate: records the existence of a relationship between A and B. For example, a note about why exercise is related to physical health could be recorded in the note *Exercise-Relate-Health*.
- Compare: records information that compares the differences between A and B. For example, a comparison of the difference between potatoes and sweet potatoes could be recorded in the note *Potatoes - compare - (sweet potatoes)*.
- Impact: records the impact of A on B. For example, information about how a teacher influences a student could be recorded in the note *Teacher-Impact-Student*.
- Apply: Record how A is applied to B. For example, content about how mathematics is applied to management could be recorded in the note *Mathematics-Applied-Management*.

It is Important to note that A and B can be concepts or entities, or even relationships. And, there can be more than two objects in the relationship, e.g. "A-B-C-Compare". Also, how you choose these four names is entirely up to you. For the same information, different people may use different titles.

## 2. 步骤

### 1. Putting information in notes


Having understood the above concepts, the next thing we need to do is to write down the information in the corresponding notes according to the following rules:

1) For information that discusses a concept or entity in a comprehensive way, we write it down in the corresponding concept note or entity note.
2) For information that discusses an aspect of a concept or entity, we write it down in the corresponding concept note or entity note, and then create subheadings in that note. 需要注意的是，有时讨论某个概念某方面的主题也会是一个独立的概念，比如“土豆烹饪”虽然是土豆的一方面，但它可以成为单独的概念笔记，因此我们要把这些内容独立出来。
3) For information that discusses a relationship between A and B, we jot it down in the corresponding relationship note and also link the current relationship note in the concept note or entity note involved in that relationship, for instance `[[A]] -> [[A-compare-B]] <- [[B]]`. Of course, very often the relationship between A and B is very simple, e.g. `A's father is B`. In this case, it is not necessary to create a special relationship note, instead we can just use a link. For example, in note A: `A's father is [[B]]`.

It is important to note that when taking notes, we need to indicate the source of the information through the pandoc reference syntax.

The following GIF shows the entire process in a more visual way.

![Pasted image 20221007203325](Attachments/Pasted%20image%2020221007203325.gif)

### 2. 收尾

1. 链接潜在链接
2. 拆分内容
3. 归档。选择一种分类法对笔记进行归类。这一方面避免未来同一文件夹下过多文件而造成系统卡顿，也给未来 的检索提供新的角度（分类检索）。当然这一步并不是必要的。

## 3. 一些注意事项

上文中的信息可以是摘录也可以是想法。因此，kg法是一种个人信息组织方法，更侧重如何组织信息，而不是告诉你应该记什么。

另外，我们可以随意创建概念笔记，但需要概念笔记的名称能够汇聚信息。一般来说，大家都用的概念肯定可以创建概念笔记。而一些只有你自己使用的概念同样也可以创建概念笔记，毕竟这是你自己的知识管理系统。因此，创建概念笔记的核心是概念笔记能汇聚一些信息。

# Ⅲ. Examples of features

综上，KG 笔记法具有知识融合、高效检索和简单推理三个特点，接下来本库将对这三个用法进行进一步说明。

## 知识融合

知识融合是高效检索的前提，也是个人知识管理系统和图书馆最大的区别。毕竟讲述同一个主题的书可以由不同的作者出版成百上千本，但对于个人来说，一个主题的知识就应当汇聚在一起，方便我们后期利用时一次性检索完全。由于 KG 笔记法以严格控制的标题为检索符号，因此我们在记录新知识时能很方便地将同一个主题的知识内容记录到同一篇笔记上，从而把相同主题的知识融合在一起。

比如，无论是现在还是未来，当我看了关于“父母心理控制”的文章，想摘抄原文或产生了新想法新洞见时，我都能轻松地找到《父母心理控制》这篇笔记，将摘录或灵感登记于其上，方便我后续检索利用。

![[Pasted image 20221007193220.png]]

## 高效检索

与侧重于搜索的方法不同，KG 法将工作重心前移到了组织环节，将严格控制的标题作为检索符号，以降低后期检索的复杂性。

比如，当我想要进一步查找“父母心理控制”相关内容时，我只需要在 Obsidian 的快速切换中输入“父母心理控制”即可定位到相关笔记，并在该笔记中通过小标题进一步定位所需信息。而当我想查找“父母心理控制和外化问题行为之间的关系的时候”，我只要输入“父母心理控制-关系-外化问题行为”即可定位到相关笔记。（你们也可以试试）

![[Pasted image 20221006143631.gif]]

当然，很多时候一个概念不会只有一个名称。因此，KG 法进一步借鉴了叙词语言的词形控制和词义控制思想，利用 Obsidian 的别名来解决概念的多名称问题。比如查找父母心理控制相关内容，我也可以使用“psychological control”这一英文概念名称。

![[Pasted image 20221006145129.gif]]
最后，如果我重读了笔记中的内容但仍然无法理解时，我可以通过笔记末尾的 pandoc 引用语法 `[@citekey, page]`，使用 [Quicker动作](https://getquicker.net/Sharedaction?code=d76ca089-0769-4a61-8a63-08d916bcf619) 快速跳转回原文献 PDF，从而结合上下文进一步回忆理解笔记内容。

![[Pasted image 20221006145916.gif]]

## 知识推理

KG 法的另一特征就是将标题作为语义化的检索符号，结合知识图谱的思想，从而能一定程度上基于笔记内容对潜在关系进行推理。

比如，当我需要写一篇关于“父母控制是否会导致孩子焦虑”的论文时，我可以通过 Path-finder 插件检索以《父母控制》这篇笔记为起点、以《焦虑》这篇笔记为终点的路径图。

![[Pasted image 20221006150351.gif]]

如结果所示， Path-finder 插件为我绘制了十余条可能的路径。


![[Pasted image 20221006102437.png]]

接下来我需要做的，只需要判断哪条路径在逻辑上最为可行即可。并且，由于 KG 法知识融合的特性，每篇笔记都汇聚了所有关于其标题的内容，因此我不必再打开文献库查找原始文献，而只需要打开路径上的笔记即可对路径进行深入研究。

![[Pasted image 20221006150723.png]]

# 三、场景示例：应用 KG 法于写作

在 KG 法的帮助下，使用笔记输出文章就变得比较具有实际操作性了：

1. 可以在大脑中或 Obsidain 中随意漫游节点，想想看哪两个节点可能存在关联。
2. 使用 Path-finder 来计算这两个节点间的潜在逻辑路径。
3. 在计算结果中找到我们觉得逻辑上最为可行的那条路径。
4. 阅读路径上经过的笔记，进一步研究这条路径是否切实可行。
5. 将路径代表的逻辑转换为文章。文章所需要使用的引文可从笔记中直接获取，一般无需重新翻阅文献库。
6. 利用 Pandoc 排版，并自动生成参考文献，
7. 发表/发布文章。

# 未来与展望

示例到这里就结束了。其实将 Obsidian 用于知识管理和知识输出并不是门槛极高的事，并不需要我们把插件商店的六百多个插件研究透彻，关键在于我们是否真的去记录和管理了我们的知识。

当然，从理论上来说，KGnotes 也有着自己的限制：

1）三元组理论本身就不适合表达非常复杂的主题。所以在实践中对于复杂主题我们一般只能用最简单的标题去概括。（对于这个限制，如果你了解知识图谱相关知识并有更好的解决办法，欢迎联系我！）
2）与知识图谱一样，知识的推理需要还要较大的节点与联系才能实现。

不过，从我7k余篇笔记的实践来看，以上限制并不太影响我们日常使用。根据以往学员的反馈，本方法平均练习记录几十篇笔记后即可上手。如果在使用中遇到了疑惑，或是想将方法应用到自己所从事的领域，欢迎通过[Obsidian 中文论坛](https://forum-zh.obsidian.md/u/ryooo/summary)、[知乎](https://www.zhihu.com/people/rao-yao-47-68)或 [邮箱](kgnotes@163.com) 联系我，我会和你一同探索。
