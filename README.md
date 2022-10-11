This is a demo vault for [KG Notes](https://forum-zh.obsidian.md/t/topic/2059) (Knowledge Graph Notes). This vault will explain the creation and basic use of KG Notes. To experience the full feature, you need to use this vault with the [path-finder](https://github.com/jerrywcy/obsidian-path-finder) plugin (which is installed in this vault).

(sorry for my poor English. If you know Chinese, you can read [Chinese Version](https://github.com/11-check-it-out/KGnotes-demo).)

# I. Introduction

## 1. The origin: what do we really need?

I'm sure many of you, are wondering how to use note taking software, or what the notes can give us.

This question has been bothering me ever since taking notes. I had pinned my hopes on note-taking software, hoping that it would tell me the answer. So over the past few years, I have switched to different note-taking software — Evernote, OneNote, Notion, RoamResearch, Obsidian. Every software has told me that I should build my own second brain, that I should generate new insights from my notes. But how to do this? The softwares didn't tell me the answer.

Thus, I saw this as a methodological problem and turned my attention to various note-taking methods. I hoped that these methods would turn my note-taking software into my second brain and allow me to generate new inspiration from my notes. From the original Luhmann Note Box, to the Zettlekasten, to the later series of methods based on them, I have used each of these methods one by one. More than the note taking software itself, these methods are really teaching me how to organise my notes and how to get new ideas out of them. But I still found it a little bit confusing because these methods were more focused on delivering ideas without giving rigorous steps that could be taken to build a personal system of notes -- they were more about telling me the reason and the vision for doing so. When I tried to understand how to build my own system of knowledge, I was always told: "Everyone's system of knowledge is different, you can't copy me, you have to learn from my ideas and build your own system". However, after six months of studying, I couldn't figure it out. So I started to look for a more operational approach.

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

## 2. Procedure

### 1. Putting information in notes


Having understood the above concepts, the next thing we need to do is to write down the information in the corresponding notes according to the following rules:

1) For information that discusses a concept or entity in a comprehensive way, we write it down in the corresponding concept note or entity note.
2) For information that discusses an aspect of a concept or entity, we write it down in the corresponding concept note or entity note, and then create subheadings in that note. It is important to note that sometimes a topic that discusses an aspect of a concept can also be a separate concept. For example, although 'potato cooking' is an aspect of potatoes, it can also be considered as a separate concept, so we should write about it in a separate concept note.
3) For information that discusses a relationship between A and B, we jot it down in the corresponding relationship note and also link the current relationship note in the concept note or entity note involved in that relationship, for instance `[[A]] -> [[A-compare-B]] <- [[B]]`. Of course, very often the relationship between A and B is very simple, e.g. `A's father is B`. In this case, it is not necessary to create a special relationship note, instead we can just use a link. For example, in note A: `A's father is [[B]]`.

It is important to note that when taking notes, we need to indicate the source of the information through the pandoc reference syntax.

### 2. Wrapping up

Again, there are three steps here: 

1. Spotting potential relationships. After taking the information into the relevant notes, we also look for missing or potential relationships in the notes. If there is a simple relationship, such as `A's mother is C`, we link the related concept or entity using square brackets, like `A's mother is [[C]]`. If there is a complex relationship, we create a relationship note and extract the relevant content into the relationship note.
2. Splitting up separate concepts. As mentioned earlier, as more content is recorded under a subheading in the concept notes and we learn more about it, we may find that it is actually also a unique concept or we may see it as a concept ourselves. Therefore, we need to separate out this section as well. My potato cooking method, for example, may not be a concept for you, but I can think of it as a unique concept called *ryooo's potato cooking method*.
3. Classifying and archiving. Finally, we need to choose a taxonomy for the archiving of the notes taken. Dewey Decimal Classification, Library of Congress Classification, para, any classification will be fine. On the one hand, this is to avoid future system lag caused by too many files in the same folder, and on the other hand it gives a new perspective for future searches ( classification searches). This step is not necessary, however.

The following GIF shows the entire process in a more visual way.

![Pasted image 20221007203325](Attachments/Pasted%20image%2020221007203325.gif)

## 3. Some things to keep in mind

The 'information' in the above can be either extracts from articles or your own unique ideas. The KG notes method is therefore a way of organising personal information, focusing more on how to organise the information rather than telling you what information should be written down. (I don't actually think this is something that knowledge organisations should be concerned with.)

In addition, the naming of concept notes is relatively arbitrary, as the essence of concept notes is to use the title as a retrieval symbol for the content in the notes. Therefore, this retrieval symbol we can either use a commonly accepted concept name or our own habitual concept name, as long as we ourselves know which information the symbol refers to.

# Ⅲ. Examples of features

In summary, the KG notes method is characterised by three features: knowledge integration, efficient retrieval and simple deduction, and these three usages will be further explained in this vault.

## 1. Knowledge integration

Knowledge integration is a precondition for efficient retrieval and is the biggest difference between a personal knowledge management system and a library. After all, hundreds of books on the same subject can be published by different authors, but for the individual, knowledge on a single subject should be brought together so that we can easily retrieve it all at once when we need it.

For example, now and in the future, when I read an article about "Parental Psychological Control" and want to extract the original text or have a new idea about this topic, I can easily find the note Parental Mind Control" and record the extract or inspiration on it, which I can easily retrieve and use later.

![](Attachments/Pasted%20image%2020221007193220.png)

## Efficiently search

In contrast to search-focused methods, the KG notes method moves the focus forward to organisation, using strictly controlled titles as retrieval symbols to reduce the complexity of searches.

For example, when I want to find out more about "parental psychological control", I simply type `parental psychological control` into Obsidian's quick switcher so that I can find the relevant note. Then I can use the outline of this note to find the information I need in the corresponding subheadings. When I want to find information about "The impact of parental psychological control on externalising problem behaviour", I just type in `(parental psychological control) - impact - (externalising problem behaviour)` to locate the relevant note. (You can try this too)

![](Attachments/Pasted%20image%2020221006143631.gif)

Of course, very often a concept does not have only one name. Therefore, the KG notes method further draws on the ideas of morphological control and lexical control in subject terms, using Obsidian aliases to solve the problem of multiple names for concepts. For example, if I were to look up parental psychological control, I could also use the Chinese concept name '父母心理控制'.

![](Attachments/Pasted%20image%2020221006145129.gif)

Finally, if I reread something in my notes but still can't understand it, I can use the pandoc reference syntax `[@citekey, page]` at the end of my notes to use [Quicker action](https://getquicker.net/Sharedaction?code=d76ca089-0769 -4a61-8a63-08d916bcf619) to quickly jump back to the original PDF to further understand the notes in context.

![](Attachments/Pasted%20image%2020221006145916.gif)

## Knowledge deduction

Another feature of the KG notes method is the use of titles as semantic retrieval symbols, combined with the idea of knowledge graphs, thus enabling a certain degree of deduction of potential relationships based on the content of the notes.

For example, when I need to write a paper on "Does parental control cause anxiety among children", I can use the Path-finder plugin to create a path map starting with the note *Parental control* and ending with the note *Anxiety*.

![](Attachments/Pasted%20image%2020221006150351.gif)

As you can see, the Path-finder plugin drew more than ten possible paths for me.

![](Attachments/Pasted%20image%2020221011211426.png)

All I had to do next was to determine which path was the most logically possible. And, thanks to the knowledge integration characteristic of the KG notes method, each note brings together all the content about its title. So instead of opening the literature management software to find the original literature, I can simply open the notes on the paths and do a deeper dive into the paths.

![](Attachments/Pasted%20image%2020221011211543.png)

# IV. Example scenario: applying the KG notes method to writing

With the help of the KG notes method, it becomes more operational to use notes to produce articles:

1. Feel free to roam around the nodes in your brain or in Obsidain to see which two nodes might be related.
2. Use Path-finder to calculate a potential logical path between these two nodes.
3. Find the path that we feel is most logically feasible from the results of the calculation.
4. read the notes passed on the path to further investigate whether this path is feasible.
5. Translate the logic represented by the path into an article. The citations needed for the article can be obtained directly from the notes and there is usually no need to go back through the literature management software.
6. using Pandoc to layout and automatically generate references.
7. publish the article in a journal or blog.

# V. Prospect

This is the end of the example. In fact, it is not difficult to use Obsidian for knowledge management and knowledge production, we don't need to study the 600+ plugins in the plugin shop thoroughly, the key is whether we have actually recorded and managed our knowledge.

In theory, of course, KG notes method has its own limitations.

1) The triplet theory itself is not suitable for expressing very complex topics. So in practice, we can only use the simplest titles to summarise complex topics. (If you know anything about knowledge graphs and have a better solution to this limitation, please contact me!)
2) As with knowledge graphs, knowledge deduction requires a large number of nodes and connections to achieve.

Overall, however, from my practice of over 7,000 notes, the above limitations do not affect our daily use too much. According to feedback from other users, this method can be mastered after practising taking a few dozen notes on average. If you encounter doubts in using it, or would like to apply the method to your own field, please feel free to contact me, and I will explore with you.
