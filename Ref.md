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
<div class="colorscripter-code" style="color:#010101; font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; position:relative !important; overflow:auto"><table class="colorscripter-code-table" style="margin:0; padding:0; border:none; background-color:#fafafa; border-radius:4px;" cellspacing="0" cellpadding="0"><tr><td style="padding:6px; border-right:2px solid #e5e5e5"><div style="margin:0; padding:0; word-break:normal; text-align:right; color:#666; font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; line-height:130%"><div style="line-height:130%">1</div><div style="line-height:130%">2</div></div></td><td style="padding:6px 0"><div style="margin:0; padding:0; color:#010101; font-family:Consolas, 'Liberation Mono', Menlo, Courier, monospace !important; line-height:130%"><div style="padding:0 6px; white-space:pre; line-height:130%">var&nbsp;test&nbsp;=&nbsp;'test';</div><div style="padding:0 6px; white-space:pre; line-height:130%">console.log('test:',&nbsp;test);</div></div></td><td style="vertical-align:bottom; padding:0 2px 4px 0"><a href="http://colorscripter.com/info#e" target="_blank" style="text-decoration:none; color:white"><span style="font-size:9px; word-break:normal; background-color:#e5e5e5; color:white; border-radius:10px; padding:1px">cs</span></a></td></tr></table></div>
</code>
