# 关于公众号问需金山中你呼我应功能的改进建议
# 探究缘起
作为社区服务类的公众号，常常会遇到关注度不高，办事效率低等问题。因此我们想通过调查，设计可行的改进措施，让社区服务类公众号依托数据，完成技术的革新。本研究以问需金山公众号为例，旨在通过调查其中你呼我应的数据来提高办事效率，提高公众号关注度。研究发现问需金山中“你呼我应”板块虽然有较大使用次数，但近期出现使用次数减少的问题。同时，我们通过研究2022年8至12月的数据，发现其中包含了许多重复提交的或者是社区公告类型的诉求，这些问题，让我们发现了改进你呼我应的可能性。

本文利用你呼我应的后台数据，通过Python等软件进行数据分析和处理，尝试对各类问题做深入调查并利用Python进行适当归类，对于结果采用图像、图表等可视化处理方法，并对现状提出意见。通过研究，我们建议限制同一用户短时提交次数，避免无效使用，耗费人力；而公众号宣传方式较为单一，大规模的涨粉源于疫情期间必要的信息登记，宣传效益并不好，为此我们希望公众号能公示部分普遍诉求的解决过程，增加活跃用户个数以及民众幸福感；最后则是通过数据分析，关键词检索等技术来对诉求解决的优先级进行排序以提升办事效率，通过以上几点提出改进措施。

# 一、研究方法
## （一）明确研究对象
  明确方向后，第一个问题是研究对象的选择。我们关注到问需金山这一公众号。由于这一公众号起步不久，可运用的技术和可改进的地方也相对较多，因此我们以你呼我应2022年8至12月的诉求数据为参考，提出一些可以应用在问需金山公众号的运营上的新思路。
## （二）资料查询
### ①民呼我应类公众号的“公示”功能
1、问需金山使用情况：在最近办结中公开了部分问题的解决过程，有处置现场的照片，但是否公开是公众号自行决定。

2、国内同行“随申办”使用情况：类似的民呼我应板块，公开了许多居民提交的诉求，居民可以自己选择是否让自己的诉求被公示，提升事件曝光度。
### ②关于公众号的关注度
1、我们注意到问需金山涨粉的主要契机是疫情期间必要的信息登记，因此这种短时间的大幅度涨粉并不能代表宣传工作的成功，在疫情信息登记之后，活跃的用户可能在其中微乎其微。
<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div>                            <div id="fc8f68d0-d4a0-4a86-ab07-a961b07ee1cf" class="plotly-graph-div" style="height:100%; width:100%;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("fc8f68d0-d4a0-4a86-ab07-a961b07ee1cf")) {                    Plotly.newPlot(                        "fc8f68d0-d4a0-4a86-ab07-a961b07ee1cf",                        [{"hovertemplate":"\u65e5\u671f=%{x}<br>\u7d2f\u79ef\u5173\u6ce8\u4eba\u6570=%{y}<extra></extra>","legendgroup":"","line":{"color":"#636efa","dash":"solid"},"marker":{"symbol":"circle"},"mode":"markers+lines","name":"","orientation":"v","showlegend":false,"x":["11\u67084\u65e5","11\u67085\u65e5","11\u67086\u65e5","11\u67087\u65e5","11\u67088\u65e5","11\u67089\u65e5","11\u670810\u65e5","11\u670811\u65e5","11\u670812\u65e5","11\u670813\u65e5"],"xaxis":"x","y":[3427,5178,11708,21508,31215,39287,40661,44151,44724,44731],"yaxis":"y","type":"scatter"}],                        {"legend":{"tracegroupgap":0},"template":{"data":{"barpolar":[{"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"barpolar"}],"bar":[{"error_x":{"color":"#2a3f5f"},"error_y":{"color":"#2a3f5f"},"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"bar"}],"carpet":[{"aaxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"baxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"type":"carpet"}],"choropleth":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"choropleth"}],"contourcarpet":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"contourcarpet"}],"contour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"contour"}],"heatmapgl":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmapgl"}],"heatmap":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmap"}],"histogram2dcontour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2dcontour"}],"histogram2d":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2d"}],"histogram":[{"marker":{"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"histogram"}],"mesh3d":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"mesh3d"}],"parcoords":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"parcoords"}],"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatter3d"}],"scattercarpet":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattercarpet"}],"scattergeo":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergeo"}],"scattergl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergl"}],"scattermapbox":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattermapbox"}],"scatterpolargl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolargl"}],"scatterpolar":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolar"}],"scatter":[{"fillpattern":{"fillmode":"overlay","size":10,"solidity":0.2},"type":"scatter"}],"scatterternary":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterternary"}],"surface":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"surface"}],"table":[{"cells":{"fill":{"color":"#EBF0F8"},"line":{"color":"white"}},"header":{"fill":{"color":"#C8D4E3"},"line":{"color":"white"}},"type":"table"}]},"layout":{"annotationdefaults":{"arrowcolor":"#2a3f5f","arrowhead":0,"arrowwidth":1},"autotypenumbers":"strict","coloraxis":{"colorbar":{"outlinewidth":0,"ticks":""}},"colorscale":{"diverging":[[0,"#8e0152"],[0.1,"#c51b7d"],[0.2,"#de77ae"],[0.3,"#f1b6da"],[0.4,"#fde0ef"],[0.5,"#f7f7f7"],[0.6,"#e6f5d0"],[0.7,"#b8e186"],[0.8,"#7fbc41"],[0.9,"#4d9221"],[1,"#276419"]],"sequential":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"sequentialminus":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]]},"colorway":["#636efa","#EF553B","#00cc96","#ab63fa","#FFA15A","#19d3f3","#FF6692","#B6E880","#FF97FF","#FECB52"],"font":{"color":"#2a3f5f"},"geo":{"bgcolor":"white","lakecolor":"white","landcolor":"#E5ECF6","showlakes":true,"showland":true,"subunitcolor":"white"},"hoverlabel":{"align":"left"},"hovermode":"closest","mapbox":{"style":"light"},"paper_bgcolor":"white","plot_bgcolor":"#E5ECF6","polar":{"angularaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","radialaxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"scene":{"xaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"yaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"zaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"}},"shapedefaults":{"line":{"color":"#2a3f5f"}},"ternary":{"aaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"baxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","caxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"title":{"x":0.05},"xaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2},"yaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2}}},"title":{"text":"changes of numbers of cases"},"xaxis":{"anchor":"y","domain":[0.0,1.0],"title":{"text":"\u65e5\u671f"}},"yaxis":{"anchor":"x","domain":[0.0,1.0],"title":{"text":"\u7d2f\u79ef\u5173\u6ce8\u4eba\u6570"}}},                        {"responsive": true}                    )                };                            </script>        </div>
2、 我们通过分析近四个月的诉求总数，发现诉求数正在不断的下降。在疫情过后，你呼我应作为公众号中最重要的部分之一，理应投入更多的精力。然而之前关于你呼我应的宣传推文反响并不好，阅读量很低，得到关注度少。

## （三）实际数据
###  ①关于无效信息
在你呼我应板块，我们总共有463个你呼我应的数据，其中官方的通知有146个；同时，我们通过筛选电话号以及姓名查到36条重复的诉求。这两类无效信息在总共的你呼我应诉求中占比39.3%。无效信息占比大，对于处理诉求的工作人员是一种负担。
 
###  ②关于类似诉求
我们在总共的463条数据中，发现了其中有很多高频出现的词语，如图所示（这里需要 比如共享单车，垃圾 词条占比的统计图）。基于此，我们发现通过关键词检索，可以对事件进行快速分类并分配到负责人，大大提高了工作效率。同时，这也可以为工作人员解决问题的优先级提供建议，我们可以选择优先解决社区公共事务，然后将这些诉求的解决过程和结果通过公众号推文的形式公示，从而让民众看到工作人员在努力解决他们的普遍需求，久而久之形成良好口碑，这样关注量也会随之上涨。

# 二、改进措施
## （一）关于提高处理诉求效率：
研究发现，诉求中关于垃圾处理，车辆停放两类问题的比例非常之大，分别占据了百分之巴拉巴拉。同时我们也发现，这两类问题的处理方法其实也非常简单，基本只需要联系相应社区的物业或者保安等人员即可。如此以来，我们便思考，是不是可以在后台加入一些关键词的筛选功能，从而对处理事件的人员进行自动分配呢？例如天骄苑热心群众上报了一例垃圾未处理的情况，系统此时检索到垃圾这一关键词，便会自动分配给天骄苑物业进行处理，这样以来便大大减少了人工处理的过程。即使在未来用户数量大幅度提高的情况下，后台人员仍然有能力处理更多的诉求。如果在未来关键词有所变化，我们也可以根据最新数据对新关键词
## （二）关于减少垃圾消息：
## （三）关于提高用户数量和你呼我应知名度：
