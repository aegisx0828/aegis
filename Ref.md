Ref Document
=============
> ###### Markdown ref : https://gist.github.com/ihoneymon/652be052a0727ad59601#23-목록
Solr Project 
-------------
* 공식 홈페이지 http://lucene.apache.org/solr/
* 위키 https://wiki.apache.org/solr/FrontPage
* 컨플루언스 https://cwiki.apache.org/confluence/display/solr/About+This+Guide
1. solr 디렉토리 구조
> http://dev-b.blogspot.kr/2012/10/apache-solr-3-enterprise-search-server.html

2. solrcloud 시 sqlconfig.xml 위치
> 참고 사이트 : https://stackoverflow.com/questions/30093340/cannot-find-proper-solrconfig-xml-file-for-configuration-in-solr-5-1-0

> ../solr-5.1.0/server/solr/configsets/data_driven_schema_configs **해당 위치에 존재함**
<code>
<div class="colorscripter-code" style="color:#f0f0f0; font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; position:relative !important; overflow:auto"><table class="colorscripter-code-table" style="margin:0; padding:0; border:none; background-color:#272727; border-radius:4px;" cellspacing="0" cellpadding="0"><tr><td style="padding:6px; border-right:2px solid #4f4f4f"><div style="margin:0; padding:0; word-break:normal; text-align:right; color:#aaa; font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; line-height:130%"><div style="line-height:130%">1</div><div style="line-height:130%">2</div><div style="line-height:130%">3</div><div style="line-height:130%">4</div><div style="line-height:130%">5</div><div style="line-height:130%">6</div></div></td><td style="padding:6px 0"><div style="margin:0; padding:0; color:#f0f0f0; font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; line-height:130%"><div style="padding:0 6px; white-space:pre; line-height:130%"><span style="color:#f0f0f0">&lt;</span><span style="color:#ff3399">html</span><span style="color:#f0f0f0">&gt;</span></div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#f0f0f0">&lt;</span><span style="color:#ff3399">head</span><span style="color:#f0f0f0">&gt;</span><span style="color:#f0f0f0">&lt;</span><span style="color:#f0f0f0">/</span><span style="color:#ff3399">head</span><span style="color:#f0f0f0">&gt;</span></div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#f0f0f0">&lt;</span><span style="color:#ff3399">body</span><span style="color:#f0f0f0">&gt;</span></div><div style="padding:0 6px; white-space:pre; line-height:130%"><span style="color:#f0f0f0">&lt;</span><span style="color:#ff3399">input</span>&nbsp;<span style="color:#a8ff58">type</span>=<span style="color:#ffd500">"text"</span><span style="color:#a8ff58"></span><span style="color:#f0f0f0">&gt;</span></div><div style="padding:0 6px; white-space:pre; line-height:130%">&nbsp;&nbsp;&nbsp;&nbsp;<span style="color:#f0f0f0">&lt;</span><span style="color:#f0f0f0">/</span><span style="color:#ff3399">body</span><span style="color:#f0f0f0">&gt;</span></div><div style="padding:0 6px; white-space:pre; line-height:130%"><span style="color:#f0f0f0">&lt;</span><span style="color:#f0f0f0">/</span><span style="color:#ff3399">html</span><span style="color:#f0f0f0">&gt;</span></div></div></td><td style="vertical-align:bottom; padding:0 2px 4px 0"><a href="http://colorscripter.com/info#e" target="_blank" style="text-decoration:none; color:white"><span style="font-size:9px; word-break:normal; background-color:#4f4f4f; color:white; border-radius:10px; padding:1px">cs</span></a></td></tr></table></div>
</code>
