# Suggestions on improving the function of "you ask,I answer" in official account
#  Introduction 
As a public account of community service, it often encounters problems of low attention and low efficiency. Therefore, we want to design feasible improvement measures through investigation, so that the public account of community service can rely on data to complete the technological innovation. This study takes the public account of "wenxujinshan" as an example, aiming to improve the working efficiency and the attention of the public account by investigating the data of "you ask, I answer". Our study found that although the "you ask, I answer" section in the account has been used for many times, the usage decreased recently. At the same time, by looking at the data from August to December 2022, we found that it contained a lot of repeated submissions or community announcement type appeals, which opened up the possibility of improving the account.

This paper makes use of the background data of "you ask, I answer", conducts data analysis and processing through Python and other software, attempts to conduct in-depth investigation of various problems and properly classify them by using Python, adopts visualization processing methods such as images and charts for the results, and puts forward suggestions on the status quo. Through research, we suggest limiting the number of short-time submission by the same user to avoid invalid use and manpower consumption; However, the publicity method of the public account is relatively simple. The large increase of fans is due to the necessary information registration during the epidemic period, and the publicity benefit is not good. Therefore, we hope that the public account can publicize the solution process of some common appeals, so as to increase the number of active users and the happiness of the public. Finally, data analysis, keyword retrieval and other technologies are used to sort the priority of the appeal solution to improve efficiency.


# Method
## I.Identify the research object
  Once the direction is clear, the first problem is the choice of research objects. We pay attention to ask need Kingsoft this public number. Since this official account has not long started and there are relatively many technologies and improvements that can be applied, we put forward some new ideas that can be applied to the operation of the official account of QDemand Kingsoft based on the appeal data from August to December 2022.
## II.Data inquiry
### ①The "publicity" function of public account
1、the condition of "wenxujinshan" ：The official account has disclosed some of the process of solving the problem, including photos of the disposal site, but it is up to the official account to decide whether to disclose it.

2、similar official account "suishenban"：Many appeals submitted by residents were made public, and residents could choose whether to have their appeals publicized to increase the visibility of the incident.
### ②About the attention of the public number
1、We have noticed that the main reason for the increase of users is the registration of information necessary during the epidemic period. Therefore, such a short and large increase in users does not represent the success of the publicity work. After the registration of the epidemic information, the number of active users may be very small.
<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div>                            <div id="fc8f68d0-d4a0-4a86-ab07-a961b07ee1cf" class="plotly-graph-div" style="height:100%; width:100%;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("fc8f68d0-d4a0-4a86-ab07-a961b07ee1cf")) {                    Plotly.newPlot(                        "fc8f68d0-d4a0-4a86-ab07-a961b07ee1cf",                        [{"hovertemplate":"\u65e5\u671f=%{x}<br>\u7d2f\u79ef\u5173\u6ce8\u4eba\u6570=%{y}<extra></extra>","legendgroup":"","line":{"color":"#636efa","dash":"solid"},"marker":{"symbol":"circle"},"mode":"markers+lines","name":"","orientation":"v","showlegend":false,"x":["11\u67084\u65e5","11\u67085\u65e5","11\u67086\u65e5","11\u67087\u65e5","11\u67088\u65e5","11\u67089\u65e5","11\u670810\u65e5","11\u670811\u65e5","11\u670812\u65e5","11\u670813\u65e5"],"xaxis":"x","y":[3427,5178,11708,21508,31215,39287,40661,44151,44724,44731],"yaxis":"y","type":"scatter"}],                        {"legend":{"tracegroupgap":0},"template":{"data":{"barpolar":[{"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"barpolar"}],"bar":[{"error_x":{"color":"#2a3f5f"},"error_y":{"color":"#2a3f5f"},"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"bar"}],"carpet":[{"aaxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"baxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"type":"carpet"}],"choropleth":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"choropleth"}],"contourcarpet":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"contourcarpet"}],"contour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"contour"}],"heatmapgl":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmapgl"}],"heatmap":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmap"}],"histogram2dcontour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2dcontour"}],"histogram2d":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2d"}],"histogram":[{"marker":{"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"histogram"}],"mesh3d":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"mesh3d"}],"parcoords":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"parcoords"}],"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatter3d"}],"scattercarpet":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattercarpet"}],"scattergeo":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergeo"}],"scattergl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergl"}],"scattermapbox":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattermapbox"}],"scatterpolargl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolargl"}],"scatterpolar":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolar"}],"scatter":[{"fillpattern":{"fillmode":"overlay","size":10,"solidity":0.2},"type":"scatter"}],"scatterternary":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterternary"}],"surface":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"surface"}],"table":[{"cells":{"fill":{"color":"#EBF0F8"},"line":{"color":"white"}},"header":{"fill":{"color":"#C8D4E3"},"line":{"color":"white"}},"type":"table"}]},"layout":{"annotationdefaults":{"arrowcolor":"#2a3f5f","arrowhead":0,"arrowwidth":1},"autotypenumbers":"strict","coloraxis":{"colorbar":{"outlinewidth":0,"ticks":""}},"colorscale":{"diverging":[[0,"#8e0152"],[0.1,"#c51b7d"],[0.2,"#de77ae"],[0.3,"#f1b6da"],[0.4,"#fde0ef"],[0.5,"#f7f7f7"],[0.6,"#e6f5d0"],[0.7,"#b8e186"],[0.8,"#7fbc41"],[0.9,"#4d9221"],[1,"#276419"]],"sequential":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"sequentialminus":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]]},"colorway":["#636efa","#EF553B","#00cc96","#ab63fa","#FFA15A","#19d3f3","#FF6692","#B6E880","#FF97FF","#FECB52"],"font":{"color":"#2a3f5f"},"geo":{"bgcolor":"white","lakecolor":"white","landcolor":"#E5ECF6","showlakes":true,"showland":true,"subunitcolor":"white"},"hoverlabel":{"align":"left"},"hovermode":"closest","mapbox":{"style":"light"},"paper_bgcolor":"white","plot_bgcolor":"#E5ECF6","polar":{"angularaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","radialaxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"scene":{"xaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"yaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"zaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"}},"shapedefaults":{"line":{"color":"#2a3f5f"}},"ternary":{"aaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"baxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","caxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"title":{"x":0.05},"xaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2},"yaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2}}},"title":{"text":"changes of numbers of cases"},"xaxis":{"anchor":"y","domain":[0.0,1.0],"title":{"text":"\u65e5\u671f"}},"yaxis":{"anchor":"x","domain":[0.0,1.0],"title":{"text":"\u7d2f\u79ef\u5173\u6ce8\u4eba\u6570"}}},                        {"responsive": true}                    )                };                            </script>        </div>

<div>                            <div id="2badbf14-a730-4d75-8f99-73c20552a2c6" class="plotly-graph-div" style="height:100%; width:100%;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("2badbf14-a730-4d75-8f99-73c20552a2c6")) {                    Plotly.newPlot(                        "2badbf14-a730-4d75-8f99-73c20552a2c6",                        [{"hovertemplate":"\u65e5\u671f=%{x}<br>\u603b\u8bbf\u95ee\u91cf=%{y}<extra></extra>","legendgroup":"","line":{"color":"#636efa","dash":"solid"},"marker":{"symbol":"circle"},"mode":"markers+lines","name":"","orientation":"v","showlegend":false,"x":["11\u67083\u65e5","11\u67084\u65e5","11\u67085\u65e5","11\u67086\u65e5","11\u67087\u65e5","11\u67088\u65e5","11\u67089\u65e5","11\u670810\u65e5","11\u670811\u65e5","11\u670812\u65e5","11\u670813\u65e5","11\u670814\u65e5","11\u670815\u65e5"],"xaxis":"x","y":[3320,2693,812,2876,6250,6372,1891,348,609,13014,869,193,123],"yaxis":"y","type":"scatter"}],                        {"legend":{"tracegroupgap":0},"template":{"data":{"barpolar":[{"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"barpolar"}],"bar":[{"error_x":{"color":"#2a3f5f"},"error_y":{"color":"#2a3f5f"},"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"bar"}],"carpet":[{"aaxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"baxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"type":"carpet"}],"choropleth":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"choropleth"}],"contourcarpet":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"contourcarpet"}],"contour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"contour"}],"heatmapgl":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmapgl"}],"heatmap":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmap"}],"histogram2dcontour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2dcontour"}],"histogram2d":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2d"}],"histogram":[{"marker":{"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"histogram"}],"mesh3d":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"mesh3d"}],"parcoords":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"parcoords"}],"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatter3d"}],"scattercarpet":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattercarpet"}],"scattergeo":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergeo"}],"scattergl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergl"}],"scattermapbox":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattermapbox"}],"scatterpolargl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolargl"}],"scatterpolar":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolar"}],"scatter":[{"fillpattern":{"fillmode":"overlay","size":10,"solidity":0.2},"type":"scatter"}],"scatterternary":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterternary"}],"surface":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"surface"}],"table":[{"cells":{"fill":{"color":"#EBF0F8"},"line":{"color":"white"}},"header":{"fill":{"color":"#C8D4E3"},"line":{"color":"white"}},"type":"table"}]},"layout":{"annotationdefaults":{"arrowcolor":"#2a3f5f","arrowhead":0,"arrowwidth":1},"autotypenumbers":"strict","coloraxis":{"colorbar":{"outlinewidth":0,"ticks":""}},"colorscale":{"diverging":[[0,"#8e0152"],[0.1,"#c51b7d"],[0.2,"#de77ae"],[0.3,"#f1b6da"],[0.4,"#fde0ef"],[0.5,"#f7f7f7"],[0.6,"#e6f5d0"],[0.7,"#b8e186"],[0.8,"#7fbc41"],[0.9,"#4d9221"],[1,"#276419"]],"sequential":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"sequentialminus":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]]},"colorway":["#636efa","#EF553B","#00cc96","#ab63fa","#FFA15A","#19d3f3","#FF6692","#B6E880","#FF97FF","#FECB52"],"font":{"color":"#2a3f5f"},"geo":{"bgcolor":"white","lakecolor":"white","landcolor":"#E5ECF6","showlakes":true,"showland":true,"subunitcolor":"white"},"hoverlabel":{"align":"left"},"hovermode":"closest","mapbox":{"style":"light"},"paper_bgcolor":"white","plot_bgcolor":"#E5ECF6","polar":{"angularaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","radialaxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"scene":{"xaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"yaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"zaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"}},"shapedefaults":{"line":{"color":"#2a3f5f"}},"ternary":{"aaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"baxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","caxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"title":{"x":0.05},"xaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2},"yaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2}}},"title":{"text":"changes of numbers of cases"},"xaxis":{"anchor":"y","domain":[0.0,1.0],"title":{"text":"\u65e5\u671f"}},"yaxis":{"anchor":"x","domain":[0.0,1.0],"title":{"text":"\u603b\u8bbf\u95ee\u91cf"}}},                        {"responsive": true}                    )                };                            </script>        </div>

* data source：问需金山公众号后台2022年11月日访问量统计

2、 我们通过分析近四个月的诉求总数，发现诉求数正在不断的下降。在疫情过后，你呼我应作为公众号中最重要的部分之一，理应投入更多的精力。然而之前关于你呼我应的宣传推文反响并不好，阅读量很低，得到关注度少。
<div>                            <div id="8353104d-915d-46a8-935d-e3950f59608f" class="plotly-graph-div" style="height:100%; width:100%;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("8353104d-915d-46a8-935d-e3950f59608f")) {                    Plotly.newPlot(                        "8353104d-915d-46a8-935d-e3950f59608f",                        [{"hovertemplate":"Month=%{x}<br>Numbers of cases=%{y}<extra></extra>","legendgroup":"","line":{"color":"#1F77B4","dash":"solid"},"marker":{"symbol":"circle"},"mode":"markers+lines","name":"","orientation":"v","showlegend":false,"x":["September","October","November","December"],"xaxis":"x","y":[204,156,81,26],"yaxis":"y","type":"scatter"}],                        {"legend":{"tracegroupgap":0},"template":{"data":{"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"width":3},"marker":{"size":9},"type":"scatter3d"}],"scattergeo":[{"line":{"width":3},"marker":{"size":9},"type":"scattergeo"}],"scattergl":[{"line":{"width":3},"marker":{"size":9},"type":"scattergl"}],"scatterpolargl":[{"line":{"width":3},"marker":{"size":9},"type":"scatterpolargl"}],"scatterpolar":[{"line":{"width":3},"marker":{"size":9},"type":"scatterpolar"}],"scatter":[{"line":{"width":3},"marker":{"size":9},"type":"scatter"}],"scatterternary":[{"line":{"width":3},"marker":{"size":9},"type":"scatterternary"}],"table":[{"cells":{"height":30},"header":{"height":36},"type":"table"}]},"layout":{"font":{"size":18},"xaxis":{"title":{"standoff":15}},"yaxis":{"title":{"standoff":15}}}},"title":{"text":"changes of numbers of cases"},"xaxis":{"anchor":"y","domain":[0.0,1.0],"title":{"text":"Month"}},"yaxis":{"anchor":"x","domain":[0.0,1.0],"title":{"text":"Numbers of cases"}}},                        {"responsive": true}                    )                };                            </script>        </div>

* 数据来源：8-12月你呼我应使用量


# Result 研究结果
##  I.关于无效信息
在你呼我应板块，我们总共有462个你呼我应的数据，其中官方的通知有146个；同时，我们通过筛选电话号以及姓名查到37条重复的诉求。这两类无效信息在总共的你呼我应诉求中占比39.61%。无效信息占比大，对于处理诉求的工作人员是一种负担。
 
## II.关于类似诉求
我们在总共的462条数据中，发现了其中有很多高频出现的词语，如图所示，因此根据关键词对于诉求进行初步的分类和处理是有一定的可行性的。
<div>                            <div id="8bac28ff-285e-40ca-ac6d-200febab2a9b" class="plotly-graph-div" style="height:100%; width:100%;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("8bac28ff-285e-40ca-ac6d-200febab2a9b")) {                    Plotly.newPlot(                        "8bac28ff-285e-40ca-ac6d-200febab2a9b",                        [{"domain":{"x":[0.0,1.0],"y":[0.0,1.0]},"hovertemplate":"high- frequency words=%{label}<br>occurrence=%{value}<extra></extra>","labels":["others","cars and shared bikes","rubbish","occupy the road"],"legendgroup":"","name":"","showlegend":true,"values":[68,59,137,11],"type":"pie"}],                        {"legend":{"tracegroupgap":0},"template":{"data":{"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"width":3},"marker":{"size":9},"type":"scatter3d"}],"scattergeo":[{"line":{"width":3},"marker":{"size":9},"type":"scattergeo"}],"scattergl":[{"line":{"width":3},"marker":{"size":9},"type":"scattergl"}],"scatterpolargl":[{"line":{"width":3},"marker":{"size":9},"type":"scatterpolargl"}],"scatterpolar":[{"line":{"width":3},"marker":{"size":9},"type":"scatterpolar"}],"scatter":[{"line":{"width":3},"marker":{"size":9},"type":"scatter"}],"scatterternary":[{"line":{"width":3},"marker":{"size":9},"type":"scatterternary"}],"table":[{"cells":{"height":30},"header":{"height":36},"type":"table"}]},"layout":{"font":{"size":18},"xaxis":{"title":{"standoff":15}},"yaxis":{"title":{"standoff":15}}}},"title":{"text":"high frequency words"}},                        {"responsive": true}                    )                };                            </script>        </div>
* 数据来源：8-12月中天社区你呼我应诉求统计

## III.关于提高处理诉求效率：
研究发现，诉求中关于垃圾处理，车辆停放两类问题的比例非常之大，分别占据了百分之巴拉巴拉。同时我们也发现，这两类问题的处理方法其实也非常简单，基本只需要联系相应社区的物业或者保安等人员即可。如此以来，我们便思考，是不是可以在后台加入一些关键词的筛选功能，从而对处理事件的人员进行自动分配呢？例如天骄苑热心群众上报了一例垃圾未处理的情况，系统此时检索到垃圾这一关键词，便会自动分配给天骄苑物业进行处理，这样以来便大大减少了人工处理的过程。即使在未来用户数量大幅度提高的情况下，后台人员仍然有能力处理更多的诉求。如果在未来关键词有所变化，我们也可以根据最新数据对新关键词
## IV.关于减少垃圾消息：
经调查研究发现，从2022年8月30日至2022年12月14日的462条“你呼我应”中，可以被明确证明是同一用户在短时间内发送多条重复“你呼我应”的信息有37条（以电话号码作为判断依据），而疑似是同一用户在短时间内发送多条重复“你呼我应”的信息（以发送信息时间、地点和每条信息之间的重复度作为判断依据）有41条，总占比达16.88%。由上可知，垃圾信息在“你呼我应”板块中也具有一定的比例，减少此类重复的垃圾信息也能在一定程度上减轻工作人员的负担。

由此，我们提出以下解决方案：首先是设置一天内提交次数的上限（3-5次左右），以防同一用户重复提交信息；二是在每次提交之间设置间隔时间（大约半小时左右），以防某用户的“刷屏”行为造成不必要的负担。
## V.关于提高用户数量和你呼我应知名度：
在用户基数庞大的支持下，你呼我应使用数仍然不高的根本原因是知名度不够，用户对其信任度也不足。由于大多数用户是为了登记疫情信息而关注问需金山公众号，所以我们的想法是：如何将这一大部分流量转换为你呼我应的流量？于是我们决定以小部分人群的优质体验作为推广手段，让你呼我应形成良好的口碑。我们发现，在便民服务的最下面有你我呼应的最近办结事项的反馈。这一些是管理人员选择公示出来的部分，但存在两个问题： 
### ① 地方太隐蔽不容易被发现 
### ② 公示内容太少，信服力不足。
因此，我们建议将公示板块融入你呼我应板块，用户可以在点击进入你呼我应进行上报时，看到以往的办理过程和办理结果并可以自主选择是否将处理过程公开。同时，后台人员可以定期挑选一些优质的办理结果，进行美化处理后通过推文的形式发布。在疫情即将过去的当下，问需金山也需要更多的推文和更多种类的公益方式来维持运营，如此一来就为问需金山提供了更多的丰富公众号内容的方式。
# Discussion 展望
在疫情即将过去的今天，问需金山公众号依靠疫情获得的流量和关注会越来越少，转型势在必行。你呼我应作为居民和社区的沟通渠道，也必将承担更多的任务，成为公众号的主要业务。以上是对你呼我应功能的一点研究和发现，希望能有所帮助。祝你呼我应在未来能开发出更多的便民功能，更好的实现服务于民。
