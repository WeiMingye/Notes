# 总论
首先请允许我自我介绍一下，我的名字叫 Sergei Garcia，我是一名拥有两年工作经验的全职前端开发工程师，之前在福布斯500强咨询公司和小公司都工作过。这对大多数人来说可能没什么，但对我意味着职业生涯上的里程碑。我两年之前除了在网上学过一点点C#和Java以外，没有任何的编程经验，没读过计算机专业的学位，并且也没有去过培训班。

之前我在许多网络社区里汲取了很多营养，获得了很多帮助。现在也该是我写一些东西分享给大家的时候了。虽然我并不是什么大神，但我想通过了解我的这些经历，至少能帮你少走一些弯路。

如果你比较着急，想要快速了解如何从零开始成为一名前端工程师的话，也可以跳过只看：最佳捷径 这个章节。

废话不多说，进入正题：

掌握基础

在我刚打算开始学习前端开发时，想到的第一个问题就是“我到底该学些什么？”。在网上搜了搜，我发现大部分初学者都在关注以下几个知识点：

JavaScript
HTML & CSS
CSS 预处理器(Less & Sass)
响应式设计
JS框架
设计模式
Git
NodeJS
自动化构建工具
JavaScript

我是在CodeSchool（付费）和Codecademy（免费）上开始学习JavaScript的。有人可能不了解这两个网站，他们都属于交互式学习的平台，可以一边看视频一边读教程，然后在浏览器就可以编写代码通过测验。我觉得对初学者来说这是最友好的学习方式。

在我掌握了一些基础之后，就开始阅读 Eloquent Javascript: A Modern Introduction to Programming这本书（你可以点击链接获取免费的在线英文版，也可以在JavaScript编程精解找到中文版）。网上很多人向我推荐这本教程，最早学习阅读它的时候是很痛苦的，不过我很庆幸我坚持了下来。这本书很棒，因为它涵盖了JS的方方面面。

假如你对jQuery感兴趣也可以去学学，不过我推荐先放到之后再说。

HTML&CSS

之后我按照CodeSchool的HTML&CSS 学习路径学习了HTML&CSS的基础知识。同样值得推荐的还有Codecademy的HTML&CSS课程，另外Udacity的HTML和CSS简介可能相对更深入一些。

P.S. Jon Duckett 所著的 HTML & CSS设计与构建网站也是学习入门HTML/CSS的一本非常棒的高分热销书。

LESS/SASS

Less & Sass 一类的CSS预处理器在CSS之上添加许多有用的特性，你可以通过这些预处理器使用CSS原生不支持的高级功能，然后再将它们编译成为CSS。

目前主流的CSS预处理器有Less & Sass两种。Sass可能更受欢迎一些，Less也挺好用的，它上手需要安装的依赖更少一些。你也可以先直接体验一下：在WinLess’s Online Less Compiler你可以在线编写Less代码，并且有一些示例供你参考；在SassMeister你可在线体验Sass.

Less或者Sass你想先学哪个都可以，它们都有很多相似之处。想了解更多可以查看Comparison between LESS & SASS

响应式设计

关于学习响应式设计，Udacity的Responsive Web Design Fundamentals课程非常不错。

假如你还能学习了解一下Bootstrap的话，上手响应式设计应该会更快一些，它的官方文档就是一个很好的开始的地方。

AngularJS

如果你想要了解AngularJS到底是什么，可以观看Google开发者的视频Design Decisions in AngularJS.

刚开始学习Angular的时候我就打算在它的官网读读文档，可惜那文档写的一点都不友好，晦涩难懂。Codeschool上有关AngularJS的课程也不怎么样，内容设置勉强合理，但代码答题的环节有很多Bug，我明明写对的答案就是无法通过测验。

最后我终于找到了一个很棒的网站Egghead.io，它的课程把Angular拆分成一个个小的知识点，每个2-5分钟就可以学完。（网站同样提供React/Node等JS相关教程）

设计模式

事实上设计模式就是一些在编程开发中解决共性问题的经验总结。这方面的知识在所有编程语言之间是通用的，同样也有助于让你写出别人更易读懂的代码，你也能更好地理解别人。

我找到了两个比较好的教程JavaScript Design Patterns和Learning JavaScript Design Patterns.

这里有中文版的JavaScript设计模式，只可惜普遍评价翻译的奇烂无比，要是你对英文不自信，那就只好忍耐一下了。

Chrome开发者工具

这应该是对前端开发者最有用的工具之一了，掌握学习它非常有必要。你可以在Codeschool的Explore and Master Chrome DevTools课程学习。

Git（版本控制系统）

最早我不了解Git的时候以为根本没有学它的必要。Git可以记录你对代码的每一次改动，要是你有什么地方写错了，也可以很方便地退回到任意一个版本（其实版本控制对所有人都非常有用，试想你在改稿改到第十版的时候，老板说他突然觉得还是第一版最好，结果你只保存了最后一版的心情吧）。Try Github是一个了解Git非常好的教程，Atlassian’s Git training可以让你对Git有更深入的了解。最后Codeschool的Git Learning Path也是学习Git非常不错的参考。

NodeJS

掌握NodeJS对一名前端开发者来讲非常有帮助。NodeSchool.io是一个学习Node非常好的地方。

自动化构建工具(Grunt&Gulp)

我自己从来都想不到还有像Grunt和Gulp这样神奇的工具。简单来讲，这些自动化构建工具可以通过脚本自动完成一些任务。例如将Less/Sass编译成为CSS形式。而且你可以设置构建工具监听你对代码的修改，每次修改完成后自动编译，你直接就可以在浏览器里看到实时的效果。这节约了大量的开发时间。

学习使用Grunt和Gulp都需要你了解NodeJS的相关知识，相比Grunt来讲，Gulp更容易配置一些，我也推荐你学习Gulp，当然这全在于你的个人喜好。

你可以在http://Scotch.io上学习Grunt和Gulp.

我在第一份工作中遇到的困难和挑战

在我掌握了这些前端开发的基础之后，我已经有了应聘前端初级岗位的能力。全靠我扎实的JavaScript基础，我才找到了第一份工作。在接下来的一年里，我仍然在继续努力提升自己。

我的第一个项目就需要开发可复用的Web组件，这令我感到很紧张。我当时犯过的错误主要有两个：

1.害怕失败。因为我只是个新人，我很怕自己的代码写错或写的太烂，所以我浪费很多时间重复地检查，确保自己没有犯错并使用了最佳实践。这也导致我固步自封，没办法掌握新的东西或创造性地实现需求。

2.盲目效仿。我当时经常会盲目效仿那些比我有经验的人。也不去思考别人为什么那么做，代码为什么那么写。我也效仿相同的做法是因为我觉得他们都比我有经验，而不去了解这些最佳实践背后的意义和原因。

感谢我的项目主管最终帮我克服了这些。他不断地鼓励我尝试新的东西，即使有时候会出错；也鼓励我多思考多质疑。最后我学到了很多东西，也明白了这些最佳实践是怎么总结出来的。

在项目中应用AngularJS对我来说也是一大挑战，因为很多东西我都只是会用而已，AngularJS就是这么神奇，无法解释其背后的原理。我几次也都想要了解其背后的工作原理，可是那些文档实在是太难懂。直到我后来找到了一本非常棒的书Build Your Own AngularJS.我只是读了Scopes和Watchers章节，就让我很好地了解了angular的工作机制。

一年之后我遇到的挑战是Web开发的迅猛发展。我正在沾沾自喜掌握了AngularJS和Grunt，Gulp和ReactJS就火了起来。等我又花了一年功夫学习之后，Webpack又开始流行。自己掌握的知识过气并不是一件令人舒服的事情。后来，我的一位同事的观点改变了我的看法：

框架和库也许会过时，但是它们背后的原理和概念会经受住时间的考验。

完全正确。AngularJS也许有些过时了，可是理解它例如Directives背后的原理也有助于理解React的组件。

除此之外，我在随后的项目中没有遇到过太大的困难。在我学习前端开发这两年里，最重要的一点是保持热情不断学习新的东西。前端的发展变化实在是太快了。

另外一方面，明白有些东西可以不去学对于一名前端开发者的成长也非常重要。很多人都抱怨前端技术的革新异常迅猛，几乎每天都有新的JS框架和库推出。最后我也终于明白：

你并不需要学习和掌握所有的框架和库。

也许你可以尝试每个框架的Hello wrold示例，但通常你只需要专注于最好和最适用于你自己的，或者手头的项目需要的就好。在层出不穷的框架中间抉择真的不是易事，好在我们能够在网上找到相当多的这类讨论。

进阶提高

再然后，我又通过下面这些方法继续学习和提升：

JavaScript

读完Eloquent JavaScript之后，你以为你掌握了JavaScript，但是You Don’t Know JS这套书会摧毁你的这种自信。我的资深前端同事向我推荐了好几次这套书，直到我真的一页页翻开了这套书，我才了解到JS究竟有多复杂，还有许多没有彻底了解JS时会踩的坑。

阅读这套书确实开启了我的思路，我同样也推荐给那些自以为很了解JS的人读一读。随后，这里还有两个很棒的学习资料：

JavaScript, The Better Parts: 来自D. Crockford 的演讲，主要涵盖了JS最大的缺点，优点，以及如何利用它们。
The Two Pillars of JavaScript: 来自 Eric Eliott的一篇文章，主要讲解了JS的两大要点——原型继承和函数式编程。
在你对JS有了一个深刻的认识之后，尝试着学习JS的最新标准ECMASCript 2015 (a.k.a. ES6)吧。这有一篇非常棒的介绍ES6的文章ECMAScript 6 (ES6): What’s New In The Next Version Of JavaScript，你也可以直接在浏览器里尝试一下ES6语法Babel’s online transpiler.

CSS

CSS的代码很容易就会变得非常凌乱。想要写出条理清晰的CSS有很多种解决方案，我在这里强烈推荐两种比较好的：

SMACSS: CSS的可扩展模块化架构。适用于各种大小级别的站点。
BEM: 一种实现前端模块代码复用的标准方案。
我个人比较喜欢SMACSS，因为它看起来更清晰一点，但也有很多公司在实践中使用BEM标准。

同样，你也需要开始关注CSS的性能了，这有两篇文章： Managing Mobile Performance Optimization和 High Performance Animation 都可以帮助你理解入门。

JavaScript构建工具

到这一步你应该以及很熟悉Grunt/Gulp了，接下来就需要把JS的构建工具加入到你的自动化构建工具中，以此来更好地管理组织你的JS代码。目前最流行的两个是：

Browserify: 打包你JS的模块化代码使其得以在浏览器中运行。
Webpack: 这是一个更高级的构建工具，除了JS以外还能管理构建CSS代码甚至是图片一类的静态资源，就是配置起来比较复杂。
http://Scotch.io上的一个小教程Getting Started with Browserify可以让你快速入门Browserify，Why Can’t Anyone Write a Simple Webpack Tutorial是入门Webpack的一个非常棒的教程。我自己并不经常使用Webpack，它虽然配置复杂，但用起来还是非常爽的。最新的流行趋势就是Webpack.

ReactJS

ReactJS越来越受欢迎，而且火得一发不可收拾。甚至有人开始讨论“React要灭掉Angular了吗？”。http://Scotch.io上的教程Learning React.js: Getting Started and Concepts可以让你对React有一个完整直观的印象。之后你可以跟着React Fundamentals教程试着开发一个React的App，当然你也可以查阅React官方文档。

由于React只注重于视图的实现，同时我也推荐你学习Redux，大多数的Redux教程都比较复杂，CSS Tricks Leveling Up with React: Redux这一篇还算深入浅出地讲解了Redux。当然你也可能听说过Flux，要是你很难在它们之间抉择的话可以查看这一篇讨论Why use Redux over Facebook Flux.

P.S 当然还有别的流行框架可以学习： Vue刚刚发布了2.0版本，学习Vue可以查看作者本人的新手向：Vue 2.0 的建议学习顺序。 学习React可以从中文文档开始。

回顾我所犯的错及从中总结的经验

在学习前端开发的两年里我犯了许多错，最严重地一点是，在我基础还不扎实地时候就开始使用框架和库了。我想这种情况应该在学习任何语言时都可能会遇到，不过对于JS尤其突出。因为JS真的是一个充满了坑地语言。

在我学习AngularJS地时候曾经遇到了一个有关$scope的Bug，我用了3天都没搞明白怎么回事。最后才发现了并不是Angular的毛病，而是因为我对JS本身的this原理理解不够导致的。

代码工整

我很少看到有关这个话题的讨论，刚开始的时候我并不在意自己的代码是否工整。大多数人都是在抱怨自己之前写的代码有多脏多烂。那么为什么就没人讲讲他们之前写得干净工整的代码呢？

我希望这种情况能够得到改善，这需要我们每个人的努力。努力写出含义明确的变量名，即使你需要多打几个字母。否则你只能在之后加上注释来解释清楚，而到了最后别人甚至你自己都很难读懂那些代码是什么意思。所以从现在开始改变吧。

写出干净工整的代码也能够让你的同事更愿意与你合作，也会让你在工作生活中更顺心一些。

jQuery

有人可能注意到了，我没怎么提到jQuery.因为在我的实际经验中，jQuery对我的害处更大一些，你可能不太理解，请听我解释：在我刚开始学习的时候，我感觉jQuery可以被应用在任何地方，解决任何问题。所以我几乎在所有地方都是用jQuery，一旦遇到了任何问题，就去寻找使用jQuery的解决办法。不要误解我的意思，jQuery确实很棒，实在好用的有些过分，所以也就让我忽视了，在我写的jQuery代码中有90%其实可以用很简单的原生JS实现。

你现在可能会想：jQuery也不是什么重量级框架，而其你可以用比原生JS少很多的代码实现一些功能，用它到底有什么不对呢？确实，使用jQuery而不是原生代码并不是主要的问题。而是我在实现一些功能时必须依赖jQuery才能想到解决方法。而这在我接手一些不使用jQuery的项目中当然就成为了很严重的问题。使用jQuery让我对它产生了严重的依赖，也让我几乎了解不到一些JS的原生功能。我掌握的这些方法脱离了jQuery根本就无法使用。

在那以后，我就强迫自己尽量不去使用jQuery，除非是在一些需要大量操作DOM的情况下。再强调一遍，我不是说jQuery不好，但假若我有一次从头再来的机会的话，我一定会先学习如何脱离jQuery来开发，而不是依赖于它。要是你现在也遇到相同的麻烦，可以看这篇You Might Not Need jQuery.

教程资源

CodeSchool
HTML/CSS一类的基础教程很不错。
Team Treehouse
教程的质量相当不错，你可以免费试用，不过试用期后每月是30刀袄。
egghead.io - Learn professional JavaScript tools with Tutorial Videos & Training
关于付费教程

确实，有些人不花一分钱学习编程可以得到那些花了钱的人一样的学习效果。我在前面列出的学习资源里大部分是免费的当然也有付费的。有些东西确实还是在视频里有人手把手教你好理解一些。

没错，很多付费的教程的确也非常糟糕，我之前就买到过。但像Egghead.io, CodeSchool, Team Treehouse这些网站上的教程非常棒，通过这些系统的教程学习1-2个月，比起你在良莠不齐博客和文章里学习效率要高太多。

付费教程并不是必须的，但我想你只要是没穷到那份儿上，选择一些优质的付费教程还是对你非常有帮助的。

成功秘笈

在过去两年里，我见过许多的开发者。但是很少遇到比较杰出的，让他人仰慕的开发者。我总觉出这类人都有一些通共的特点，这也是成为一名成功的前端开发者的秘籍：

热爱你的工作。这是最重要的一点特质。要是你根本不喜欢写代码，代码也不会喜欢你。在一个领域杰出的人往往是对其所在充满热情的人。
大方地分享你的知识。你也许很想把自己解决一些问题的代码保密，但请别这么做。乐于分享他知识的人往往是最有价值的人，因为他们可以进入任何一个团队并带领团队进步。
跟紧潮流趋势。不管是阅读博客，还是参与编程问题的讨论，甚至是在休息时谈论前端开发的话题，跟紧潮流趋势也会让你保持领先的位置。
最佳捷径

也许你对我的经历和碎碎念并不感兴趣，所以我在这里提供了这个学习资源的列表：

Javascript

CodeSchool 或 Treehouse’s Javascript learning path (付费) 或 Codecademy’s Javascript course.
Eloquent JavaScript
You Don’t Know JS
JS: The Right Way
Learn ES6 by Egghead.io
HTML & CSS

CodeSchool 或 Treehouse’s HTML & CSS learning path(付费) 或 HTML and CSS: Design and Build Websites by John Ducket 或 Codecademy’s HTML & CSS course.
Specifics on CSS Specifity by CSS Tricks
Learn CSS Layout
SMACSS
9 basic principles of responsive web design by Froont
Responsive Web Design Fundamentals by Google on Udacity (如果你没看过 CodeSchool 或 Treehouse learning path)
Managing Mobile Performance Optimization by Smashing Magazine 或 Browser Rendering Optimization 以及 Website Performance Optimization by Google on Udacity.
Web fundamentals by Google
Developer Tools

Explore and Master DevTools by CodeSchool
Learn Git by Codecademy 和 Try Github by Codeschool
Introduction to Linux Commands by Smashing Magazine
Automate Your Tasks Easily with Gulp.js by Scotch.io
AngularJS

Design Decisions in AngularJS by Google Developers (介绍 AngularJS)
AngularJS fundamentals by Egghead.io
John Papa’s Angular Styleguide
Creating a Single Page Todo App with Node and Angular (MEAN) by Scotch.io
AngularJS application structure by Egghead.io (Paid) OR Scotch.io’s Angular Courses
ReactJS

Learning React.js: Getting Started and Concepts by Scotch.io
Intro to webpack by Egghead.io
React Fundamentals by Egghead.io
Leveling Up with React: Redux by CSS Tricks
Back End

NodeJS tutorials by NodeSchool.io
How I explained REST to my Wife
Creating a Single Page Todo App with Node and Angular by Scotch.io (Node, ExpressJS, MongoDB, Angular, REST)
推荐文章

这是我自己喜欢的一些资源和文章，仅做推荐。（所以就不翻译啦，因为文章也是英文）

Web Design in 4 minutes. A very creative and original interactive tutorial that teaches you the fundamentals of web design.
Awwards. Looking for web design inspiration? Look no further.
Why Hiring is so hard in tech by Eric Eliott. Here Eric is does an amazing job at summarizing how it’s surprisingly hard to find great developers, and how to become one.
NoSQL database systems mega comparison by Kristof Kovacs. This is a superb comparison between the most popular NoSQL database systems out there. MongoDB, Redis, CouchDB, Cassandra, ElasticSearch, they and more are all here.
XSS Game. Cross-site scripting (XSS) bugs are one of the most common and dangerous types of vulnerabilities in Web applications. Using this awesome resource you can learn how to find and exploit XSS bugs, and how to prevent them from happening to your web application.
How To Write Unmaintainable Code. Hilarious article on how to NOT write maintainable, clean code.
推荐工具软件

推荐一些对我自己很有帮助的工具软件。

Jetbrains Webstorm: 超强前端IDE，学生可以免费使用。
Atom.io: Github出品的免费开源的代码编辑器。
Sublime Text: 号称最性感的编辑器。
caniuse.com: 查询浏览器的兼容性，非常好用。
Cloud 9: 提供一个在线的Linux虚拟环境，你可以在上面使用Git，Node，部署演示项目等等。
CodePen, Plunker and JSFiddle: 在线写前端代码的地方，可以实时预览，也方便分享给别人。
Vanilla List: 一个收集只使用原生JS的库（不依赖jQuery）的列表。
You Might Not Need jQuery
PublicAPIs: 所有开放的公共API
Gravit.io: 在线设计Web原型，免费袄。
Adobe Kuler:Adobe家推出的工具，用来给网站配色。
Name that color:不知道CSS某个颜色类该怎么命名？到这里来查询吧。
译者的话

原文提供的大部分资源都是英文的（其实全部是英文的，好在有些网站有中文版，我也把一些书籍替换成了中文版）。我也推荐呼吁大家使用英文资源学习。

国内的在线学习资源普遍质量实在太差，另外一定不要去培训班，或者什么付费培训群，99.999%都是骗钱的。我在这里点到为止。

如果你英文基础实在太差，请移步从零学习前端开发·目录，这里有我搜集的很多免费的在线中文学习资源。

如果你是初学者或零基础，也推荐阅读如何在一年之内通过自学找到Web开发工作。

虽然没人给我广告费，还是要再推荐一遍全世界学习Web开发最好的地方FreeCodeCamp，完全公益免费，提供安排非常详细，设计非常合理的Web开发学习路径：

官网：FreeCodeCamp
中文网：FreeCodeCampChina
有任何疑问或建议，好的学习资源分享，自己的学习经验体会等等，欢迎在评论区参与讨论。